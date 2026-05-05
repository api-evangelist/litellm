---
title: "LiteLLM release versioning is changing: standard names, MINOR for weekly, PATCH for hotfixes"
url: "https://docs.litellm.ai/blog/cleaner-release-versions"
date: "Tue, 28 Apr 2026 00:00:00 GMT"
author: ""
feed_url: "https://docs.litellm.ai/blog/rss.xml"
---
<p>LiteLLM release version names are changing. Two pain points have been driving this:</p>
<p><strong>1. The <code>-stable</code> and <code>-nightly</code> suffixes aren't standard.</strong></p>
<p>Versions like <code>v1.83.3-stable</code> and <code>v1.83.0-nightly</code> don't match PEP 440 (PyPI) or SemVer 2.0 (Docker / Helm) conventions. Users expecting standard version strings get confused, and tooling that classifies versions has to special-case the suffix.</p>
<p><strong>2. Weekly releases were bumping PATCH, leaving no room for actual hotfixes.</strong></p>
<p>Under the old model, each scheduled weekly release bumped the PATCH number: <code>1.83.0</code> -&gt; <code>1.83.1</code> -&gt; <code>1.83.2</code> -&gt; <code>1.83.3</code>. When a real hotfix was needed for <code>1.83.3</code>, the next PATCH (<code>1.83.4</code>) was already reserved for the following week's release. The workaround on Docker was <code>v1.83.3-stable.patch.1</code> - but PyPI doesn't accept that syntax, so a hotfix that needed both a Docker image and a Python wheel had no clean way to ship.</p>
<h2 class="anchor anchorWithStickyNavbar_LWe7" id="whats-new">What's new<a class="hash-link" href="https://docs.litellm.ai/blog/cleaner-release-versions#whats-new" title="Direct link to What's new">​</a></h2>
<p>Starting with <strong><code>1.84.0</code></strong>:</p>
<ul>
<li><strong>Drop the suffix.</strong> Stable releases are plain PEP 440 / SemVer 2.0: <code>1.84.0</code>. Pre-releases use the standard PEP 440 (<code>1.84.0rc1</code>, <code>1.84.0.dev42</code>) and SemVer (<code>1.84.0-rc.1</code>, <code>1.84.0-dev.42</code>) shapes for PyPI and Docker respectively.</li>
<li><strong>MINOR bumps weekly.</strong> Each scheduled stable bumps the MINOR component: <code>1.84.0</code> -&gt; <code>1.85.0</code> -&gt; <code>1.86.0</code>.</li>
<li><strong>PATCH is reserved for hotfixes.</strong> When <code>1.84.0</code> needs a fix, it becomes <code>1.84.1</code>. Cleanly installs everywhere - <code>pip install litellm==1.84.1</code>, <code>docker pull ghcr.io/berriai/litellm:1.84.1</code>.</li>
</ul>
<h2 class="anchor anchorWithStickyNavbar_LWe7" id="side-by-side">Side-by-side<a class="hash-link" href="https://docs.litellm.ai/blog/cleaner-release-versions#side-by-side" title="Direct link to Side-by-side">​</a></h2>
<table><thead><tr><th>Scenario</th><th>Old name</th><th>New name</th></tr></thead><tbody><tr><td>Weekly scheduled stable</td><td><code>v1.83.3-stable</code></td><td><code>1.84.0</code></td></tr><tr><td>Hotfix on the current stable</td><td><code>v1.83.3-stable.patch.1</code> (Docker only - no PyPI release)</td><td><code>1.84.1</code></td></tr><tr><td>Release candidate</td><td><code>v1.84.0-rc</code></td><td><code>1.84.0-rc.1</code> (Docker) / <code>1.84.0rc1</code> (PyPI)</td></tr><tr><td>Nightly</td><td><code>v1.83.0-nightly</code></td><td><code>1.84.0-dev.42</code> (Docker) / <code>1.84.0.dev42</code> (PyPI)</td></tr></tbody></table>
<p>The hotfix row is the meaningful one. Under the old scheme there was no PyPI publication for <code>v1.83.3-stable.patch.1</code>. Under the new scheme, hotfixes ship to both registries and PyPI as a normal release.</p>
<h2 class="anchor anchorWithStickyNavbar_LWe7" id="backwards-compatibility">Backwards compatibility<a class="hash-link" href="https://docs.litellm.ai/blog/cleaner-release-versions#backwards-compatibility" title="Direct link to Backwards compatibility">​</a></h2>
<p>Releases that already shipped with the old naming - <code>v1.83.x-stable</code>, <code>v1.83.x-stable.patch.N</code>, and existing <code>1.83.x</code> PyPI versions - <strong>stay on the registries and PyPI forever</strong>. Anything you currently pin to keeps working. The new naming applies to new releases starting <code>1.84.0</code>.</p>
<p>If a maintenance patch is needed on a pre-cutover release line (e.g. a fix on <code>1.83.x</code> while <code>1.84.x</code> is current), that patch may continue to use the old naming for consistency within the line - release notes will call out which format was used. Long-term, all new releases move to the new naming.</p>
<h2 class="anchor anchorWithStickyNavbar_LWe7" id="a-few-things-worth-knowing">A few things worth knowing<a class="hash-link" href="https://docs.litellm.ai/blog/cleaner-release-versions#a-few-things-worth-knowing" title="Direct link to A few things worth knowing">​</a></h2>
<ul>
<li><strong><code>litellm-dev</code></strong> - there's a separate <code>litellm-dev</code> PyPI package and <code>*-dev</code> Docker image family for ad-hoc and one-off builds (e.g. testing a fix before it lands in a release). <strong>Not for production use.</strong> Anything pinned to the standard <code>litellm</code> package or <code>ghcr.io/berriai/litellm:*</code> Docker tags will never accidentally pick up a <code>litellm-dev</code> build.</li>
<li><strong><code>:latest</code> Docker tag</strong> points to the most recent stable release on each registry, advancing automatically when a new stable ships. For production deployments we still recommend pinning to a content tag (e.g. <code>:1.84.0</code>) so deploys are reproducible.</li>
<li><strong>Image signing</strong> (<a href="https://docs.litellm.ai/blog/ci-cd-v2-improvements#verify-docker-image-signatures">cosign verify</a>) and verification commands continue to work unchanged with the new tag shapes.</li>
</ul>
