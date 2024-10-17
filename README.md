<h1>👨‍💼 Employee Information Management - MAUI App with ASP.NET Core API</h1>

<p>This project is a <strong>MAUI (Multi-platform App UI)</strong> based mobile and desktop application that performs CRUD (Create, Read, Update, Delete) operations for Employee Information, integrated with an <strong>ASP.NET Core Web API</strong> for the backend.</p>

<h2>📑 Table of Contents</h2>
<ul>
  <li><a href="#features">Features</a></li>
  <li><a href="#technologies">Technologies</a></li>
  <li><a href="#getting-started">Getting Started</a></li>
  <li><a href="#api-documentation">API Documentation</a></li>
  <li><a href="#usage">Usage</a></li>
  <li><a href="#contributing">Contributing</a></li>
  <li><a href="#license">License</a></li>
</ul>

<h2 id="features">🚀 Features</h2>
<ul>
  <li>MAUI App with Master-Detail CRUD functionality for Employee Information.</li>
  <li>Integration with ASP.NET Core Web API for managing Employee records.</li>
  <li>Cross-platform support: Android, iOS, Windows, and macOS.</li>
  <li>CRUD operations (Create, Read, Update, Delete) on employee records.</li>
  <li>REST API integration with JSON payloads.</li>
  <li>Simple, clean, and responsive UI with mobile-first design.</li>
</ul>

<h2 id="technologies">🛠️ Technologies</h2>
<ul>
  <li><strong>Frontend:</strong> .NET MAUI (Multi-platform App UI)</li>
  <li><strong>Backend:</strong> ASP.NET Core Web API</li>
  <li><strong>Database:</strong> SQL Server (or your preferred database)</li>
  <li><strong>API Documentation:</strong> Swagger/OpenAPI</li>
</ul>

<h2 id="getting-started">⚙️ Getting Started</h2>

<h3>🔧 Prerequisites</h3>
<ul>
  <li>Ensure you have the latest version of <a href="https://dotnet.microsoft.com/en-us/download/dotnet/7.0" target="_blank">.NET SDK</a> installed.</li>
  <li>Install Visual Studio 2022 with MAUI workload enabled.</li>
  <li>SQL Server or another database solution to store employee information.</li>
</ul>

<h3>📂 Clone the Repository</h3>
<pre><code>https://github.com/MdAshikur-Rahman-Ashik/MAUI_App_CoreAPI_Employee_Information
</code></pre>

<h3>Backend Setup (ASP.NET Core API)</h3>
<ol>
  <li>Navigate to the API project directory:</li>
  <pre><code>cd MAUI_EmployeeInformationManagement/Backend</code></pre>
  <li>Install dependencies and restore the project:</li>
  <pre><code>dotnet restore</code></pre>
  <li>Update your database connection string in <code>appsettings.json</code>.</li>
  <li>Apply database migrations:</li>
  <pre><code>dotnet ef database update</code></pre>
  <li>Run the API:</li>
  <pre><code>dotnet run</code></pre>
</ol>

<h3>Frontend Setup (MAUI App)</h3>
<ol>
  <li>Open the solution in Visual Studio 2022.</li>
  <li>Ensure the target platform is set correctly (Android, iOS, Windows, macOS).</li>
  <li>Build and run the MAUI app from Visual Studio.</li>
</ol>

<h2 id="api-documentation">📄 API Documentation</h2>
<p>Here are some of the available endpoints for managing employee information:</p>
<ul>
  <li><code>GET /api/employees</code> - Retrieve all employee records.</li>
  <li><code>GET /api/employees/{id}</code> - Retrieve an employee by ID.</li>
  <li><code>POST /api/employees</code> - Create a new employee record.</li>
  <li><code>PUT /api/employees/{id}</code> - Update an existing employee record.</li>
  <li><code>DELETE /api/employees/{id}</code> - Delete an employee record.</li>
</ul>
<p>For more details, refer to the API Swagger documentation once the API is running at <a href="http://localhost:5142/swagger" target="_blank">http://localhost:5142/swagger</a>.</p>

<h2 id="usage">💻 Usage</h2>
<p>Once both the API and the MAUI app are running, you can perform CRUD operations on employee records via the mobile or desktop app. The app provides an intuitive user interface for managing employees, with features like listing employees, adding new employees, editing employee details, and deleting employee records.</p>


<h2 id="contributing">🤝 Contributing</h2>
<p>Contributions are welcome! If you have suggestions or issues, feel free to open a pull request or an issue.</p>

<h2 id="license">📝 License</h2>
<p>This project is licensed under the MIT License. See the <a href="LICENSE" target="_blank">LICENSE</a> file for more details.</p>

<h2 id="network-security-configuration">🔐 Network Security Configuration</h2>
<p>The project includes a network security configuration for Android. The configuration allows cleartext traffic for the domain <code>10.0.2.2</code>.</p>

<h3>📂 Folder Structure</h3>
<pre><code>
- ProjectRoot/
  - xml/
    - network-security-config.xml
</code></pre>

<h3>📄 XML File Content</h3>
<pre><code>
&lt;network-security-config&gt;
    &lt;domain-config cleartextTrafficPermitted="true"&gt;
        &lt;domain includeSubdomains="true"&gt;10.0.2.2&lt;/domain&gt;
    &lt;/domain-config&gt;
&lt;/network-security-config&gt;
</code></pre>

<h3>🛠️ How to Use</h3>
<p>To use the configuration, place the <strong>network-security-config.xml</strong> file in the <strong>res/xml</strong> folder of your Android project and update the <strong>AndroidManifest.xml</strong> file as follows:</p>
<pre><code>
&lt;application
    android:networkSecurityConfig="@xml/network-security-config"
    ... &gt;
</code></pre>

<h2 id="dependencies">📦 Dependencies</h2>
<p>This project requires several external packages for both the API and the MAUI app. Below are instructions for ensuring all dependencies are up to date:</p>

<h3>For .NET Core API:</h3>
<ul>
  <li>To install dependencies and restore packages, run:</li>
</ul>
<pre><code>dotnet restore</code></pre>

<ul>
  <li>To update all NuGet packages to the latest version, run:</li>
</ul>
<pre><code>dotnet outdated</code></pre>

<p>To update specific NuGet packages:</p>
<pre><code>dotnet add package [PackageName] --version [VersionNumber]</code></pre>

<h3>For MAUI App:</h3>
<ul>
  <li>Install all required packages:</li>
</ul>
<pre><code>dotnet restore</code></pre>
<ul>
  <li>To update any MAUI-specific packages or tools:</li>
</ul>
<pre><code>dotnet tool update -g [toolname]</code></pre>



![Screenshot 1](https://github.com/user-attachments/assets/5503cf60-7b24-42cd-8aaa-9c67e2b31a7d)
![Screenshot 2](https://github.com/user-attachments/assets/0c3b280a-6050-4347-b06b-bfa7b95fc560)
![Screenshot 3](https://github.com/user-attachments/assets/9abcb939-df64-46ee-9873-34b194d75fd0)

