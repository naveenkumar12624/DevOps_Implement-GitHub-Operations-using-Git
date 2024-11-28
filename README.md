<h1>Aim</h1>
<p>The objective of this experiment is to guide you through the process of using Git commands to interact with GitHub, from cloning a repository to collaborating with others through pull requests.</p>

<h2>Theory</h2>
<p>GitHub is a web-based platform that offers version control and collaboration services for software development projects. It provides a way for developers to work together, manage code, track changes, and collaborate on projects efficiently. GitHub is built on top of the Git version control system, which allows for distributed and decentralized development.</p>

<h3>Key Features of GitHub:</h3>
<ul>
  <li><strong>Version Control:</strong> GitHub uses Git, a distributed version control system, to track changes to source code over time. This allows developers to collaborate on projects while maintaining a history of changes and versions.</li>
  <li><strong>Repositories:</strong> A repository (or repo) is a collection of files, folders, and the entire history of a project. Repositories on GitHub serve as the central place where code and project-related assets are stored.</li>
  <li><strong>Collaboration:</strong> GitHub provides tools for team collaboration. Developers can work together on the same project, propose changes, review code, and discuss issues within the context of the project.</li>
  <li><strong>Pull Requests:</strong> Pull requests (PRs) are proposals for changes to a repository. They allow developers to submit their changes for review, discuss the changes, and collaboratively improve the code before merging it into the main codebase.</li>
  <li><strong>Issues and Projects:</strong> GitHub allows users to track and manage project-related issues, enhancements, and bugs. Projects and boards help organize tasks, track progress, and manage workflows.</li>
  <li><strong>Forks and Clones:</strong> Developers can create copies (forks) of repositories to work on their own versions of a project. Cloning a repository allows developers to create a local copy of the project on their machine.</li>
  <li><strong>Branching and Merging:</strong> GitHub supports branching, where developers can create separate lines of development for features or bug fixes. Changes made in branches can be merged back into the main codebase.</li>
  <li><strong>Actions and Workflows:</strong> GitHub Actions enable developers to automate workflows, such as building, testing, and deploying applications, based on triggers like code pushes or pull requests.</li>
  <li><strong>GitHub Pages:</strong> This feature allows users to publish web content directly from a GitHub repository, making it easy to create websites and documentation for projects.</li>
</ul>

<h3>Benefits of Using GitHub:</h3>
<ul>
  <li><strong>Collaboration:</strong> GitHub facilitates collaborative development by providing tools for code review, commenting, and discussion on changes.</li>
  <li><strong>Version Control:</strong> Git's version control features help track changes, revert to previous versions, and manage different branches of development.</li>
  <li><strong>Open Source:</strong> GitHub is widely used for hosting open-source projects, making it easier for developers to contribute and for users to find and use software.</li>
  <li><strong>Community Engagement:</strong> GitHub fosters a community around projects, enabling interaction between project maintainers and contributors.</li>
  <li><strong>Code Quality:</strong> The code review process on GitHub helps maintain code quality and encourages best practices.</li>
  <li><strong>Documentation:</strong> GitHub provides a platform to host project documentation and wikis, making it easier to document codebases and project processes.</li>
  <li><strong>Continuous Integration/Continuous Deployment (CI/CD):</strong> GitHub Actions allows for automating testing, building, and deploying applications, streamlining the development process.</li>
</ul>

<h2>Materials</h2>
<ul>
  <li>Computer with Git installed (<a href="https://git-scm.com/downloads">Download Git</a>)</li>
  <li>GitHub account (<a href="https://github.com/">Sign up for GitHub</a>)</li>
  <li>Internet connection</li>
</ul>

<h2>Experiment Steps</h2>

<h3>Step 1: Cloning a Repository</h3>
<ol>
  <li>Sign in to your GitHub account.</li>
  <li>Find a repository to clone (you can use a repository of your own or any public repository).</li>
  <li>Click the "Code" button and copy the repository URL.</li>
  <li>Open your terminal or command prompt.</li>
  <li>Navigate to the directory where you want to clone the repository.</li>
  <li>Run the following command:
    <pre><code>git clone &lt;repository_url&gt;</code></pre>
    Replace <code>&lt;repository_url&gt;</code> with the URL you copied from GitHub.
  </li>
  <li>This will clone the repository to your local machine.</li>
</ol>

<h3>Step 2: Making Changes and Creating a Branch</h3>
<ol>
  <li>Navigate into the cloned repository:
    <pre><code>cd &lt;repository_name&gt;</code></pre>
  </li>
  <li>Create a new text file named <code>example.txt</code> using a text editor.</li>
  <li>Add some content to the <code>example.txt</code> file.</li>
  <li>Save the file and return to the command line.</li>
  <li>Check the status of the repository:
    <pre><code>git status</code></pre>
  </li>
  <li>Stage the changes for commit:
    <pre><code>git add example.txt</code></pre>
  </li>
  <li>Commit the changes with a descriptive message:
    <pre><code>git commit -m "Add content to example.txt"</code></pre>
  </li>
  <li>Create a new branch named <code>feature</code>:
    <pre><code>git branch feature</code></pre>
  </li>
  <li>Switch to the <code>feature</code> branch:
    <pre><code>git checkout feature</code></pre>
  </li>
</ol>

<h3>Step 3: Pushing Changes to GitHub</h3>
<ol>
  <li>Add Repository URL in a variable:
    <pre><code>git remote add origin &lt;repository_url&gt;</code></pre>
    Replace <code>&lt;repository_url&gt;</code> with the URL you copied from GitHub.
  </li>
  <li>Push the <code>feature</code> branch to GitHub:
    <pre><code>git push origin feature</code></pre>
  </li>
  <li>Check your GitHub repository to confirm that the new branch <code>feature</code> is available.</li>
</ol>

<h3>Step 4: Collaborating through Pull Requests</h3>
<ol>
  <li>Create a pull request on GitHub:
    <ul>
      <li>Go to the repository on GitHub.</li>
      <li>Click on "Pull Requests" and then "New Pull Request."</li>
      <li>Choose the base branch (usually <code>main</code> or <code>master</code>) and the compare branch (<code>feature</code>).</li>
      <li>Review the changes and click "Create Pull Request."</li>
    </ul>
  </li>
  <li>Review and merge the pull request:
    <ul>
      <li>Add a title and description for the pull request.</li>
      <li>Assign reviewers if needed.</li>
      <li>Once the pull request is approved, merge it into the base branch.</li>
    </ul>
  </li>
</ol>

<h3>Step 5: Syncing Changes</h3>
<ol>
  <li>After the pull request is merged, update your local repository:
    <pre><code>git checkout main 
git pull origin main</code></pre>
  </li>
</ol>

<h2>Conclusion</h2>
<p>This experiment provided you with practical experience in performing GitHub operations using Git commands. You learned how to clone repositories, make changes, create branches, push changes to GitHub, collaborate through pull requests, and synchronize changes with remote repositories. These skills are essential for effective collaboration and version control in software development projects using Git and GitHub.</p>
