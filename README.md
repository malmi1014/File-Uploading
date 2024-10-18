# File-Uploading
A file upload vulnerability occurs when a web application allows users to upload files without properly validating the type, content, or size of the uploaded file. This lack of validation can be exploited by attackers to upload malicious files, such as scripts that execute on the server. These scripts might be used to gain unauthorized access, execute code, or further compromise the server.

How File Upload Vulnerabilities Work
Unrestricted File Upload:

Some web applications allow users to upload files like images, PDFs, or documents. If there are no restrictions on the types of files that can be uploaded, an attacker could upload a script (e.g., PHP, JavaScript, or shell files).
For example, if the application only checks the file extension (e.g., .jpg or .png) but does not validate the actual file content, an attacker could upload a PHP file disguised as an image.
Lack of Server-side Validation:

Even if the client-side (browser) restricts uploads to certain file types, attackers can bypass this restriction using tools like Burp Suite. This is why server-side validation is crucial.
Arbitrary Code Execution:

When a malicious file (e.g., malicious.php) is uploaded to the server and then accessed via a URL, it can execute code on the server. For example, an attacker might upload a web shell that allows them to execute commands directly on the server.
