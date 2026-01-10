<!--
  Auto-generated file. Do not edit directly.
  Edit /home/jcook/Documents/git_repo/jcook3701.flatpak/docs/jekyll/README.md instead.
  Run ```make readme``` to regenerate this file
-->
<h1 id="flatpak">flatpak</h1>

<p><strong>Author:</strong> Jared Cook<br />
<strong>Version:</strong> 1.0.0</p>

<h2 id="overview">Overview</h2>
<p>Ansible installer for flatpak packages.</p>

<hr />

<p><img src="https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/changelog.yml/badge.svg" alt="changelog" />
<img src="https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/dependency-check.yml/badge.svg" alt="dependency-check" />
<img src="https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/format-check.yml/badge.svg" alt="format-check" />
<img src="https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/lint-check.yml/badge.svg" alt="lint-check" />
<img src="https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/security-audit.yml/badge.svg" alt="security-audit" />
<img src="https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/spellcheck.yml/badge.svg" alt="spellcheck" />
<img src="https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/tests.yml/badge.svg" alt="tests" />
<img src="https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/typecheck.yml/badge.svg" alt="typecheck" /></p>

<hr />

<h2 id="usage-examples">Usage Examples</h2>

<hr />

<h2 id="development-strategy">Development Strategy</h2>

<h3 id="️-build-environment-venv">🐍️ Build environment (.venv)</h3>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nv">$ </span>make <span class="nb">install</span>
</code></pre></div></div>

<h3 id="-dependency-management-deptry">🧬 Dependency Management (deptry)</h3>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nv">$ </span>make dependency-check
</code></pre></div></div>

<h3 id="️-security-audit-pip-audit">🛡️ Security Audit (pip-audit)</h3>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nv">$ </span>make security
</code></pre></div></div>

<h3 id="-formatting-black">🎨 Formatting (black)</h3>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nv">$ </span>make format-check
</code></pre></div></div>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nv">$ </span>make format-fix
</code></pre></div></div>

<h3 id="-linting-ansible-lint-ruff-tomllint--yaml-lint">🔍 Linting (ansible-lint, ruff, tomllint, &amp; yaml-lint)</h3>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nv">$ </span>make lint-check
</code></pre></div></div>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nv">$ </span>make lint-fix
</code></pre></div></div>

<h3 id="-spellchecking-codespell">🎓 Spellchecking (codespell)</h3>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nv">$ </span>make spellcheck
</code></pre></div></div>

<h3 id="-typechecking-mypy">🧠 Typechecking (mypy)</h3>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nv">$ </span>make typecheck
</code></pre></div></div>

<h3 id="-testing-pytest-galaxy-importer">🧪 Testing (pytest, galaxy-importer)</h3>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nv">$ </span>make <span class="nb">test</span>
</code></pre></div></div>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nv">$ </span>make galaxy-import
</code></pre></div></div>

<h3 id="-release-git-tag">🚀 Release (git tag)</h3>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nv">$ </span>make release
</code></pre></div></div>

<h3 id="-build-help">❓ Build Help</h3>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nv">$ </span>make <span class="nb">help</span>
</code></pre></div></div>

<h2 id="commit-help">Commit Help:</h2>

<p><strong>Note:</strong> Commits are required to be conventional git commit message.  This helps with the auto-generation of the changelog files and is enforced by pre-commit.</p>

<p><strong>options (default):</strong></p>

<ul>
  <li>docs</li>
  <li>chore</li>
  <li>feat</li>
  <li>fix</li>
  <li>refactor</li>
  <li>ci</li>
  <li>test</li>
  <li>perf</li>
  <li>revert</li>
  <li>build</li>
  <li>style</li>
</ul>

<p><strong>example:</strong></p>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code>&lt;<span class="nb">type</span><span class="o">&gt;[</span>optional scope]: &lt;description&gt;

<span class="o">[</span>optional body]

<span class="o">[</span>optional footer<span class="o">(</span>s<span class="o">)]</span>
</code></pre></div></div>

<ul>
  <li><code class="language-plaintext highlighter-rouge">&lt;type&gt;</code>: A required noun that describes the nature of the change.</li>
  <li><code class="language-plaintext highlighter-rouge">[optional scope]</code>: An optional phrase within parentheses that specifies the part of the codebase being affected (e.g., fix(parser):).</li>
  <li><code class="language-plaintext highlighter-rouge">&lt;description&gt;</code>: A required short, imperative-mood summary of the changes.</li>
  <li><code class="language-plaintext highlighter-rouge">[optional body]</code>: A longer description providing additional context and “what and why” details.</li>
  <li><code class="language-plaintext highlighter-rouge">[optional footer(s)]</code>: Used for adding meta-information, such as issue references (Fixes #123) or indicating breaking changes.</li>
</ul>

<hr />

<h2 id="requirements">Requirements:</h2>

<p><strong>Python 3.11</strong></p>

<div class="language-shell highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nv">$ </span><span class="nb">sudo </span>apt <span class="nb">install </span>python3.11
</code></pre></div></div>

<hr />

<h2 id="authors-notes">Author’s Notes</h2>

<h3 id="todos">TODO’s</h3>

<ol>
  <li>Documentation is currently getting wrong project_slug/name. ❌
    <ul>
      <li>Currently path for documentation is just the <code class="language-plaintext highlighter-rouge">$(project_name)</code> and not the <code class="language-plaintext highlighter-rouge">$(namespace).$(project_name)</code>.</li>
    </ul>
  </li>
  <li>Finish ci/cd for changelog generation using antsichaut ❌</li>
  <li>Create ci/cd for documentation rather than using pre-commit ❌</li>
</ol>

<hr />
