---
title: "April Townhall Updates: CI/CD v2, Stability, and Product Roadmap"
url: "https://docs.litellm.ai/blog/april-townhall-updates"
date: "Fri, 10 Apr 2026 12:00:00 GMT"
author: ""
feed_url: "https://docs.litellm.ai/blog/rss.xml"
---
<p>Thank you to everyone who joined our April town hall.</p>
<p>We used the session to share our CI/CD v2 improvements, product stability work, and what we are prioritizing next across reliability and product roadmap.</p>
<!-- -->
<h2 class="anchor anchorWithStickyNavbar_LWe7" id="cicd-v2-improvements">CI/CD v2 improvements<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#cicd-v2-improvements" title="Direct link to CI/CD v2 improvements">​</a></h2>
<p>Our CI/CD v2 work is centered around four goals:</p>
<ol>
<li><strong>Limit</strong> what each package can access</li>
<li><strong>Reduce</strong> the number of sensitive environment variables</li>
<li><strong>Avoid</strong> compromised packages</li>
<li><strong>Reduce the risk of</strong> release tampering</li>
</ol>
<h4 class="anchor anchorWithStickyNavbar_LWe7" id="new-architecture-isolated-environments">New architecture: isolated environments<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#new-architecture-isolated-environments" title="Direct link to New architecture: isolated environments">​</a></h4>
<p>We have begun moving to isolated environments for distinct CI/CD stages to reduce the chance that a single compromised step can inherit broad access across the entire pipeline.</p>
<div><svg height="348" width="640" xmlns="http://www.w3.org/2000/svg"></svg><noscript><img height="348" src="/assets/ideal-img/april_townhall_isolated_environments.31cd448.640.png" width="640" /></noscript></div>
<h4 class="anchor anchorWithStickyNavbar_LWe7" id="current-rollout-status">Current rollout status<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#current-rollout-status" title="Direct link to Current rollout status">​</a></h4>
<p>These changes are deployed in our current release workflow. <a href="https://github.com/BerriAI/litellm/tags" rel="noopener noreferrer" target="_blank">See here</a></p>
<h4 class="anchor anchorWithStickyNavbar_LWe7" id="independently-verify-releases">Independently verify releases<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#independently-verify-releases" title="Direct link to Independently verify releases">​</a></h4>
<p>A key part of CI/CD v2 is supporting independent verification of release artifacts using our published verification process, while reducing reliance on any single credential or release path.</p>
<p><a href="https://docs.litellm.ai/docs/proxy/docker_image_security" rel="noopener noreferrer" target="_blank"><strong>Learn more about how to verify releases</strong></a></p>
<div><svg height="454" width="640" xmlns="http://www.w3.org/2000/svg"></svg><noscript><img height="454" src="/assets/ideal-img/verify_releases.bda039d.640.png" width="640" /></noscript></div>
<h2 class="anchor anchorWithStickyNavbar_LWe7" id="stability-improvements">Stability improvements<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#stability-improvements" title="Direct link to Stability improvements">​</a></h2>
<h3 class="anchor anchorWithStickyNavbar_LWe7" id="sdlc-improvements">SDLC improvements<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#sdlc-improvements" title="Direct link to SDLC improvements">​</a></h3>
<p>This month, we're focusing on process stability improvements around:</p>
<ul>
<li>Improving main-branch stability</li>
<li>Mapping UI QA to built Docker images for 1:1 environment parity</li>
<li>Consistent release tags across PyPI and Docker</li>
<li>Fixing release notes publication</li>
</ul>
<h4 class="anchor anchorWithStickyNavbar_LWe7" id="improving-main-branch-stability">Improving main-branch stability<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#improving-main-branch-stability" title="Direct link to Improving main-branch stability">​</a></h4>
<p>We're introducing a staging-gated flow:</p>
<div><svg height="356" width="640" xmlns="http://www.w3.org/2000/svg"></svg><noscript><img height="356" src="/assets/ideal-img/stable_main.fc00ea2.640.png" width="640" /></noscript></div>
<ul>
<li>Only an internal staging branch can push to <code>main</code>.</li>
<li>PRs to that staging branch must pass CircleCI LLM API testing.</li>
<li>Collision handling happens on staging, which is designed to reduce unstable changes reaching <code>main</code>.</li>
</ul>
<h4 class="anchor anchorWithStickyNavbar_LWe7" id="ui-qa-in-docker-environment">UI QA in Docker environment<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#ui-qa-in-docker-environment" title="Direct link to UI QA in Docker environment">​</a></h4>
<p>Moving forward, all UI QA will be performed in the built Docker image that users run.</p>
<p>Previously, some UI QA paths were run in local environments that did not fully replicate Docker runtime conditions.</p>
<p>That contributed to release-specific issues, including MCP registration problems in <code>v1.82.3</code>.</p>
<h4 class="anchor anchorWithStickyNavbar_LWe7" id="consistent-release-tags">Consistent release tags<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#consistent-release-tags" title="Direct link to Consistent release tags">​</a></h4>
<p>Today we publish releases for multiple scenarios:</p>
<ul>
<li>Dev (Built of a PR for a customer-specific scenario)</li>
<li>Nightly (Passes all CI/CD checks)</li>
<li>Release Candidate (Passes all CI/CD checks + manual UI QA)</li>
<li>Stable (intended to pass all CI/CD checks + manual UI QA + 7 days of production testing)</li>
</ul>
<p>We are targeting a consistent naming convention across PyPI and Docker by the end of April.</p>
<h4 class="anchor anchorWithStickyNavbar_LWe7" id="release-notes">Release notes<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#release-notes" title="Direct link to Release notes">​</a></h4>
<p>CI/CD v2 changes moved release notes to a manual path. This is a temporary solution while we investigate a better automated workflow. We are targeting a more consistent process by the end of April.</p>
<h3 class="anchor anchorWithStickyNavbar_LWe7" id="product-stability-improvements">Product stability improvements<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#product-stability-improvements" title="Direct link to Product stability improvements">​</a></h3>
<h4 class="anchor anchorWithStickyNavbar_LWe7" id="stable-prisma-migrations">Stable Prisma migrations<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#stable-prisma-migrations" title="Direct link to Stable Prisma migrations">​</a></h4>
<p>Today, we have observed several migration failure classes:</p>
<ul>
<li>Migration not applied</li>
<li>Migration marked applied but incomplete</li>
<li>Migration not applied due to non-root image issues</li>
</ul>
<p>We're prioritizing this work this month and have assigned an engineering owner to the effort. Our target is to resolve these error classes by the end of April.</p>
<h4 class="anchor anchorWithStickyNavbar_LWe7" id="ui-type-safety">UI type safety<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#ui-type-safety" title="Direct link to UI type safety">​</a></h4>
<p>Another area of focus is improving the stability of the UI. Today, one cause of errors is that the UI maintains its own assumptions about backend API types. This can lead to issues when backend responses differ from UI assumptions.</p>
<p>We aim to move to having the UI and Backend be in sync with each other, and are exploring OpenAPI-driven mapping to achieve this.</p>
<h2 class="anchor anchorWithStickyNavbar_LWe7" id="product-roadmap">Product roadmap<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#product-roadmap" title="Direct link to Product roadmap">​</a></h2>
<h3 class="anchor anchorWithStickyNavbar_LWe7" id="our-assumptions">Our Assumptions<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#our-assumptions" title="Direct link to Our Assumptions">​</a></h3>
<p>Over the next few years, we expect:</p>
<ul>
<li>Companies will give employees more AI tools.</li>
<li>More AI agents will move into production workflows across HR, finance, support, and operations.</li>
</ul>
<h3 class="anchor anchorWithStickyNavbar_LWe7" id="our-inferences">Our Inferences<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#our-inferences" title="Direct link to Our Inferences">​</a></h3>
<h4 class="anchor anchorWithStickyNavbar_LWe7" id="near-term">Near-term<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#near-term" title="Direct link to Near-term">​</a></h4>
<ul>
<li>AI spend will increase.</li>
<li>Uptime and latency will become even more important.</li>
<li>More AI resources (skills, CLIs, and related assets) will require governance.</li>
<li>Agent and MCP usage patterns will require deeper controls.</li>
<li>Broader developer adoption will increase the need for simpler, more discoverable tooling.</li>
</ul>
<h4 class="anchor anchorWithStickyNavbar_LWe7" id="long-term">Long-term<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#long-term" title="Direct link to Long-term">​</a></h4>
<ul>
<li>We expect many organizations to treat agent auditability (how decisions were made across LLM + MCP + sub-agent inputs/outputs) as a compliance expectation.</li>
<li>Permission management will get more complex as user-agent interaction chains deepen.</li>
</ul>
<p>Roadmap timelines in this post are targets and may evolve based on validation and user feedback.</p>
<h2 class="anchor anchorWithStickyNavbar_LWe7" id="april-investments">April investments<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#april-investments" title="Direct link to April investments">​</a></h2>
<h3 class="anchor anchorWithStickyNavbar_LWe7" id="reliability">Reliability<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#reliability" title="Direct link to Reliability">​</a></h3>
<ul>
<li>Increase uptime for 10k+ RPS scenarios.</li>
<li>Investigate latency overhead for long-running Claude Code requests.</li>
</ul>
<h3 class="anchor anchorWithStickyNavbar_LWe7" id="feature-reliability">Feature reliability<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#feature-reliability" title="Direct link to Feature reliability">​</a></h3>
<ul>
<li>Polish MCP authentication.</li>
<li>Better understand how teams are using agents through LiteLLM.</li>
</ul>
<h3 class="anchor anchorWithStickyNavbar_LWe7" id="governance">Governance<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#governance" title="Direct link to Governance">​</a></h3>
<ul>
<li>Launch Skills as a first-class citizen in LiteLLM.</li>
</ul>
<h2 class="anchor anchorWithStickyNavbar_LWe7" id="qa">Q&amp;A<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#qa" title="Direct link to Q&amp;A">​</a></h2>
<p>Thank you again for all the questions and direct feedback. We will keep sharing concrete progress updates as these efforts ship.</p>
<h2 class="anchor anchorWithStickyNavbar_LWe7" id="hiring">Hiring<a class="hash-link" href="https://docs.litellm.ai/blog/april-townhall-updates#hiring" title="Direct link to Hiring">​</a></h2>
<p>We are actively hiring across several roles, please apply <a href="https://jobs.ashbyhq.com/litellm" rel="noopener noreferrer" target="_blank">here</a> if you're interested!</p>
