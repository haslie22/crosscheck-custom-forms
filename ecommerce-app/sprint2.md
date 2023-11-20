#### Login Page `0/130`

---

##### Input Validation `0/40`

- [ ] Implement client-side validation for the login form, including email and password fields `20/20`
  - [ ] Email field validation checks for a properly formatted email address according to the specified rules
  - [ ] Password field validation checks for meeting the length and complexity requirements
  - [ ] Show/hide password functionality allows users to toggle password visibility
  - [ ] Validation checks are performed as the user types
        &nbsp;
- [ ] Display clear error messages for validation issues `20/20`
  - [ ] Clear error messages are shown next to the corresponding input field when validation fails
  - [ ] Error messages are descriptive, explaining the specific validation issue
  - [ ] Error messages follow the specified display rules for a consistent and user-friendly experience
  - [ ] Error messages disappear when the user corrects the invalid input

---

##### Integration with Authentication Service `0/45`

- [ ] Integrate the login form with a chosen authentication service (CommerceTools) to handle user authentication `25/25`
  - [ ] CommerceTools authentication service is set up and configured for the project
  - [ ] Login form communicates with the CommerceTools authentication service to sign in users by submitting email and password
  - [ ] Application can successfully receive access token, refresh token, and user data from the CommerceTools API
        &nbsp;
- [ ] Implement error handling for failed authentication attempts using CommerceTools `20/20`
  - [ ] Clear error messages are shown when authentication fails due to incorrect email or password
  - [ ] Error messages are user-friendly and provide guidance on how to proceed
  - [ ] No sensitive information is exposed to the user in the error messages
  - [ ] The application handles CommerceTools authentication errors properly

---

##### Redirection `0/30`

- [ ] Redirect users to the application's main page upon successful login `15/15`
  - [ ] After successful authentication, users are redirected to the main page of the application, which contains simple text ("Main") or any other content
  - [ ] The URL in the address bar is changed to the main page's URL upon redirection
  - [ ] Proper handling of navigation and user experience during redirection, including browser history updates and preserving authentication state
        &nbsp;
- [ ] Redirect users who are already logged in to the main page if they try to access the login page `15/15`
  - [ ] Authenticated users who attempt to visit the login page are automatically redirected to the main page
  - [ ] The URL in the address bar is changed to the main page's URL for authenticated users redirected from the login page
  - [ ] Redirection maintains the user's authentication state during the process
  - [ ] Proper handling of navigation and user experience during redirection, including updating browser history

---

##### Handle Authentication Token `0/10`

- [ ] Obtain the authentication token securely after a successful login attempt by sending a request to the token endpoint, allowing for seamless user authentication across the application `0/10`
  - [ ] The authentication token is obtained from the token endpoint after a successful login attempt
  - [ ] The token is used for subsequent requests that require authentication

---

##### Navigation to Registration Page `0/5`

- [ ] Add a button or link on the login page that allows users to navigate to the registration page `0/5`
  - [ ] A clear and prominent button or link is present on the login page to navigate to the registration page
  - [ ] The button or link is functional and directs the user to the registration page
  - [ ] Proper handling of navigation and user experience during this process
        &nbsp;

---

#### Registration Page `0/120`

---

##### Input Validation `0/45`

- [ ] Implement client-side validation for all required fields in the registration form, such as email, password, first name, last name, date of birth, and address fields (e.g., street, city, postal code, and country) for proper use with CommerceTools `25/25`
  - [ ] Each required field in the registration form has validation rules
  - [ ] Registration form submission is prevented if the input doesn't meet the requirements
        &nbsp;
- [ ] Display clear error messages indicating any validation issues, such as an improperly formatted email or a weak password
  - [ ] Error messages are displayed for each invalid input in the registration form
  - [ ] Error messages are clear, concise, and visually accessible
  - [ ] Selected UI elements are used effectively to highlight validation errors and improve user experience

---

##### Integration with Authentication Service `0/25`

- [ ] Integrate the registration form with a chosen authentication service, such as commercetools, to handle user registration `10/10`
  - [ ] Successful user registration with the chosen authentication service
  - [ ] Proper submission of user information to the authentication service backend
  - [ ] A success message is displayed to the user upon successful account creation
  - [ ] Verification of successful customer creation using the browser's DevTools Network tab
        &nbsp;
- [ ] Implement error handling for failed registration attempts, and display user-friendly error messages `15/15`
  - [ ] Proper error handling during the registration process
  - [ ] Display user-friendly error messages for failed registration attempts
  - [ ] Selected UI elements are used effectively to highlight failed registration attempt errors and improve user experience

---

##### State Management, Automatic Login, and Redirection `0/15`

- [ ] Redirect users to the application's main page upon successful account creation and automatic login `15/15`
  - [ ] Users are redirected to the main page upon successful account creation and automatic login
  - [ ] The redirection process takes into account browser history for seamless navigation
  - [ ] Proper use of the chosen front-end framework or library for handling routing and navigation, or implementation of plain TypeScript solutions when not using a front-end framework

---

##### Integration with commercetools for User Profiles and Addresses `0/30`

- [ ] Allow users to set a default address during registration `15/15`
  - [ ] Users can set a default address while registering
  - [ ] The setting of a default address happens simultaneously with user account creation
  - [ ] The default address is saved in the user profile upon successful registration
  - [ ] Proper integration with the commercetools API for storing default address information
  - [ ] The user interface clearly distinguishes the default address selection during registration
        &nbsp;
- [ ] Enable users to select different billing and shipping addresses or choose a single address for both billing and shipping during the registration process `15/15`
  - [ ] Users can enter separate addresses for billing and shipping during the registration process
  - [ ] Users can choose to use the same address for both billing and shipping
  - [ ] The chosen addresses are saved in the user profile upon successful registration
  - [ ] The user interface clearly distinguishes between input fields for billing and shipping addresses
  - [ ] Proper integration with the commercetools API for storing billing and shipping address information

---

##### Navigation to Login Page `0/5`

- [ ] Add a button or link on the registration page that allows users to navigate to the login page `5/5`
  - [ ] The registration page includes a clear and visible button or link
  - [ ] Upon clicking the button or link, the user is redirected to the login page

---

#### Main Page Enhancements `0/65`

---

##### Centralized Navigation `0/10`

- [ ] Add links to all the functional pages of the application on the main page. These should include, but are not limited to, the login and registration pages `5/5`
  - [ ] Links to all functional pages of the application are present on the main page, including the login and registration pages
  - [ ] The links are clearly visible and accessible to users, making the navigation easy and intuitive
        &nbsp;
- [ ] Each link should redirect the user correctly to the corresponding page without any errors `5/5`
  - [ ] Each link on the main page correctly redirects to the corresponding page
  - [ ] No error occurs during the redirection process
  - [ ] The correct page content is displayed after the redirection

---

##### Routing Implementation `0/30`

- [ ] Implement routing for navigation between login, registration, and main pages `15/15`
  - [ ] Users can directly access the main page by typing its URL into the browser's address bar
  - [ ] Users can directly access the login page by typing its URL into the browser's address bar
  - [ ] Users can directly access the registration page by typing its URL into the browser's address bar
  - [ ] Direct access to these pages does not cause any errors or issues with the application's functionality
  - [ ] Navigation using the implemented routing is smooth, without page refreshes (when applicable, e.g., in a Single Page Application)
  - [ ] Navigational features of the browser (such as the back and forward buttons) work correctly after using these direct access links
        &nbsp;
- [ ] Implement a 404 (Not Found) page for invalid route requests `15/15`
  - [ ] The 404 page contains clear messaging informing the user that the requested page could not be found
  - [ ] The 404 page includes a navigation option (e.g., a button or link) for users to return to the main page or another accessible section of the application
  - [ ] The application automatically redirects users to the 404 page when they request an invalid route
  - [ ] The application should maintain the originally requested URL in the browser's address bar when showing the 404 page, as this helps support user expectations and provides clearer context about the requested route

---

##### Evaluation Criteria for Header `0/25`

- [ ] Navigation to login and registration pages for unauthorized users `15/15`
  - [ ] A clear and visible link or button for the login page is present for unauthorized users
  - [ ] Clicking the link or button takes the user to the login page
  - [ ] A clear and visible link or button for the registration page is present for unauthorized users
  - [ ] Clicking the link or button takes the user to the registration page
        &nbsp;
- [ ] Ability to access the main page for all users `5/5`
  - [ ] A navigation button or a clickable logo is present in the header that redirects users to the main page of the application
  - [ ] The navigation button or logo contains a link to the main page URL
  - [ ] Clicking on the navigation button or logo takes the user to the main page from any other page in the application.
        &nbsp;
- [ ] Logout functionality for authorized users `5/5`
  - [ ] An option to log out is available for authorized users
  - [ ] Upon logging out, users are redirected to the login or main page
  - [ ] After logging out, users have the option to log in or register again

---

#### Penalties

- [ ] Absence of Responsive Application Design `-0/20`
- [ ] Errors in the Console `-0/20`

---

#### Total: `0 / 315`
