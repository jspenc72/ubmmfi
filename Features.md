
|      Feature       |                                                  Detail                                                  |      Dependencies      | Priority |
| ------------------ | -------------------------------------------------------------------------------------------------------- | ---------------------- | -------- |
| Create Account     | - Business Owners or Business Model Managers create their own account.                                   | User Database          |        1 |
|                    | - Enrollment requires:                                                                                   | - OAuth2 API           |          |
|                    | - Username                                                                                               | - Mailer (Email)       |          |
|                    | - First and Last Name                                                                                    |                        |          |
|                    | - Email                                                                                                  |                        |          |
|                    | - Phone Number                                                                                           |                        |          |
|                    | - Password must be at least 6 characters with one non-letter character and no spaces.                    |                        |          |
|                    | - E-mail account verification                                                                            |                        |          |
| Login              | - Log in using registered username and password. Can choose to auto-store information for quicker log-in | User Database          |        1 |
|                    | - Forgot password, forgot username links to change via email when in log-in screen                       | - OAuth2 API           |          |
| Forgot Login Info  | - Type email address:                                                                                    | User Database          |        1 |
|                    | - email                                                                                                  | - OAuth2 API           |          |
|                    | - change password link or username                                                                       | - Mailer (Email)       |          |
| Login with FB      | - Facebook Oauth2 Sign-In is Required                                                                    | User Databse           |        3 |
|                    | - User will still need to create a password associated with their account                                | - OAuth2 API           |          |
|                    | - Username may be generated using user info from FB API                                                  | - FB OAuth API         |          |
| Login with G+      | - Google Oauth2 Sign-In is Required                                                                      | User Databse           |        3 |
|                    | - User will still need to create a password associated with their account                                | - OAuth2 API           |          |
|                    | - Username may be generated using user info from G                                                       | API - G Plus OAuth API |          |
| Change Log In Info | - Update e-mail address or phone #                                                                       | User Databse           |        1 |
|                    | - User should receive email and/or sms that their username or password has been changed.                 | - Mailer (Email)       |          |
