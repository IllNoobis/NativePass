# NativePass
Passkey prompt from the browser and have user sign the challenge with their passkey inside their primary browser, without the need for opening a browser environment like a custom tab, so the login feels 'native' (as if its a biometric login of the app itself)
I used the FIDO2 API with native biometrics integration, as it provides the most native-feeling experience without browser dependencies.



This implementation:

Uses a hidden WebView to handle the WebAuthn API calls
Provides a native-feeling UI without visible browser elements
Integrates with the device's native biometric system
Maintains a singleton pattern for the auth service
Includes error handling and user feedback
The solution avoids Chrome Custom Tabs while still leveraging the security of WebAuthn/passkeys. The WebView is invisible to the user, making the authentication feel completely native.

To use it, simply tap the authenticate button. The passkey prompt will appear as a native system dialog rather than a browser window.
