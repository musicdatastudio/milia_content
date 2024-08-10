## `milia_content`

### Overview
`milia_content` is a repository designed to host static content for the Milia project. This content can be accessed dynamically by various components of the Milia application, enabling the application to use up-to-date and version-controlled resources without hardcoding them into the codebase.

### Purpose
The primary purpose of `milia_content` is to provide a centralized and easily maintainable location for storing static resources such as email templates, text files, or any other content that needs to be accessed by the Milia application.

### Content Examples
- **Email Templates**:
  - `welcome_subject.txt`: Contains the subject line for the welcome email.
  - `welcome_content.html`: Contains the HTML content for the welcome email, which can include placeholders like `$EMAIL$` for personalization.

### How It Works
1. **Hosting**:
   - The content is hosted on GitHub Pages, making it publicly accessible and easy to retrieve via URLs.
  
2. **Accessing Content**:
   - The Milia application dynamically loads the content using URLs that point to specific files within the `milia_content` repository. For example:
	 - `https://static.milia.app/welcome_subject.txt` for the email subject.
	 - `https://static.milia.app/welcome_content.html` for the email body.
  
3. **Version Control**:
   - Since the content is stored in a GitHub repository, all changes are tracked, and previous versions can be restored if necessary. This allows for safer and more organized content management.

### Best Practices
- **Keep Content Updated**: Regularly update the content in the `milia_content` repository to ensure that the Milia application uses the most current information.
- **Use Placeholders**: When creating templates, use placeholders (e.g., `$EMAIL$`) to allow for easy customization within the application.
- **Version Management**: Make use of GitHub's version control to manage updates, allowing for rollbacks and tracking changes over time.

### Example Files
- **welcome_subject.txt**:
  ```plaintext
  Welcome to Milia, $EMAIL$!
  ```
  
- **welcome_content.html**:
  ```html
  <h1>Welcome to Milia, $EMAIL$</h1>
  <p>We are thrilled to have you with us!</p>
  ```

### Accessing the Repository
You can access the content directly via the following URL:
- [milia_content on GitHub Pages](https://static.milia.app/)
