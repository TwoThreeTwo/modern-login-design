## Modern Rustic Login, Sign Up, Forgot password, and main screen UI

# Features

This is a simple, modern, and easy to use UI template that is built with HTML, CSS and JavaScript. It is fully responsive and works on all devices. It is also very easy to customize and use. It is built with the latest technologies and is very fast and lightweight. 

# Screenshots
<img src="imgs/login.png" alt="">
<br>
<img src="imgs/forgotpassword.png" alt="">
<br>
<img src="imgs/signup.png" alt="">
<img src="forgotpassword.png" alt="">
<br>
<img src="signup.png" alt="">
# Installation

1. Download the files from the repository
2. Open the index.html file in your browser
3. Enjoy!

# License

This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to <https://unlicense.org>

# Contact

If you have any questions, feel free to make an issue to contact me. There will be a questions section to on GitHub issues that you can create yourself stating your question.

# Credits

- [Two](https://www.GitHub.com/twothreetwo/)
- [Unlicense](https://unlicense.org/)

# Support

Have any issues? Feel free to open an issue on the GitHub repository and I will try to fix it as soon as possible.

# Contributing

Feel free to contribute to this project by opening a pull request on the GitHub repository. I will review it and merge it if it is good.


# Todo List

- [x] Add Screenshots for: Sign up, and Forgot password screens
- [x] Check for bugs
- [x] Auto Assign labels and users for issues/features and pull requests
- [x] Fully complete issue templates
- [x] Fully complete pull request templates
- [x] Add a Pull request auto assign label and user feature
- [x] Finish Sign up screen
- [x] Finish Forgot password screen
- [x] Add google sign up button
- [x] Fix google sign up error screen
- [x] Add box shadowing to buttons
- [x] Organize CSS into sections and add comments
- [x] Include a captcha hover as a saftey provider.
- [x] Change 'login' to sign in
- [x] forgot password screen, change 'forgot password' to 'reset password'
- [x] Change 'sign up' to 'create account'
# Notes

Just so you guys know if you do wanna use this, there are a couple things to change


## Major changes you must do.

Change the DataSite Key for the google Captcha V2 Badge

``` 
                <div class="g-recaptcha"
                **data-sitekey="6Ld6ElsiAAAAAPe-eu5IS0U-ODART0K2ebCLln_9"**
                data-callback="onSubmit"
                data-size="invisible">
          </div>
```

Change this so you can link to a proper domain so the reCaptchaV2 Badge will actually work and not give you an error.

Link the Buttons to a main page, follow color pattern so it actually looks good...

Here's a script for when you want to check when someone signs in with google using the sign in btn I have created in signup.html.

                <script>
                    function onSignIn(googleUser) {
                        // Useful data for your client-side scripts:
                        var profile = googleUser.getBasicProfile();
                        console.log("ID: " + profile.getId()); // Don't send this directly to your server!
                        console.log('Full Name: ' + profile.getName());
                        console.log('Given Name: ' + profile.getGivenName());
                        console.log("Image URL: " + profile.getImageUrl());
                        console.log("Email: " + profile.getEmail());
                    
                        // The ID token you need to pass to your backend:
                        var id_token = googleUser.getAuthResponse().id_token;
                        console.log("ID Token: " + id_token);
                    }
                </script>

## Minor changes you can do.

Currently, the google sign in thing is broken, I don't really know how to fix it it just goes to the error screen, you can fix that yourself by going to google cloud and creating ur own credentials and stuff. I don't really know how to do that, so I just left it as is. 

You can also change the colors of the buttons and stuff, I just left it as is.

