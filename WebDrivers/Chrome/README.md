# Chrome WebDrivers

Via [ChromeDriver - WebDriver for Chrome](http://chromedriver.chromium.org/downloads)

## Current Releases

* If you are using Chrome version 73, please download [ChromeDriver 73.0.3683.20](./73.0.3683.20)
* If you are using Chrome version 72, please download [ChromeDriver 2.46](./2.46) or [ChromeDriver 72.0.3626.69](./72.0.3626.69)
* If you are using Chrome version 71, please download [ChromeDriver 2.46](./2.46) or [ChromeDriver 71.0.3578.137](./71.0.3578.137)
* For older version of Chrome, please see below for the version of ChromeDriver that supports it.

If you are using Chrome from Dev or Canary channel, please download [ChromeDriver 2.46](./2.46). This is not officially supported, but in most cases it should work without major issues.

> For more information on selecting the right version of ChromeDriver, please see the [Version Selection](http://chromedriver.chromium.org/downloads/version-selection) page.


### ChromeDriver 73.0.3683.20

Supports Chrome version 73

* Fixed error code returned from Execute Script command in some scenarios
* Made the HTTP server keep connection alive by default
* Fixed Close Window command to correctly handle user prompts
* Fixed error code returned while sending keys to disabled element
* Improved spec compliance of timeout value handling
* Improved spec compliance of Add Cookie command
* Increased HTTP server listening queue length
* Fixed Is Element Displayed command in v0 shadow DOM
* Added warning about Element Clear command behavior change in log file
* Fixed Execute Script command to correctly convert document.all into JSON format
* Improved handling of bad element reference
* For more details, please see the release notes.
* ChromeDriver 2.46
* Supports Chrome v71-73
* Fixed error code returned from Execute Script command in some scenarios
* Made the HTTP server keep connection alive by default
* Fixed Close Window command to correctly handle user prompts
* Fixed error code returned while sending keys to disabled element
* Improved spec compliance of timeout value handling
* Improved spec compliance of Add Cookie command
* Improved spec compliance of Switch to Frame command
* Increased HTTP server listening queue length
* Fixed Is Element Displayed command in v0 shadow DOM
* Fixed Element Double Click command
* Added warning about Element Clear command behavior change in log file
* Fixed Execute Script command to correctly convert document.all into JSON format
* Improved handling of bad element reference
For more details, please see the [release notes](https://chromedriver.storage.googleapis.com/73.0.3683.20/notes.txt).


### ChromeDriver 2.45

Supports Chrome v70-72

* Fixed New Session is not spec compliant
* Fixed ChromeDriver shouldn't launch Chrome if Chrome and ChromeDriver versions are incompatible
* Fixed Find Element command returns wrong error code when an invalid locator is used
* Fixed Some ChromeDriver status codes are wrong
* Fixed Compile error in JS inside of WebViewImpl::DispatchTouchEventsForMouseEvents
* Fixed Window size commands should handle user prompts
* Fixed ChromeDriver doesn't start Chrome correctly with Chrome option "user-data-dir="
* Fixed Status command is not spec compliant
* Fixed Add support for strictFileInteractability


### ChromeDriver 2.44

Supports Chrome v69-71

* Fixed WindowMaximize on Mac
* Fixed Incorrect 'alert open error' for window handle call
* Fixed Element Send Keys should get "text" property in W3C mode
* Fixed XML special case of Is Element Enabled is not handled as per spec
* Fixed XML special case of Get Element CSS Value is not handled as per spec
* Fixed Set Window Rect needs to check for invalid input
* Fixed Support new unhandledPromptBehavior modes


### ChromeDriver 2.43

Supports Chrome v69-71

Changes include:
* Fixed Parsing of proxy configuration is not standard compliant
* Fixed Launch app command is flaky
* Fixed Screenshot of element inside iFrame is taken incorrectly
* Added ChromeDriver supports window resizing over a remote connection
* Fixed Error codes are not handled in Clear element
* Fixed Not waiting until element is visible
* Fixed Get element property is not implemented
* Fixed Switch to Frame is not spec compliant
* Fixed Execute Async Script does not return spec compliant error codes
* Fixed Execute Script does not return spec compliant error codes
* Fixed Error code in ExecuteGet is not conformant with spec
* Fixed Send Alert Text is not returning spec compliant error codes
* Fixed clear() on an input type="date" pretends element is not user-editable
* Fixed Chromedriver gets window handle for the tab which is opened manually
* Fixed Allow append or start a new log file for chromedriver
* Fixed New Session does not invoke w3c mode if flag is in firstMatch


### ChromeDriver 2.42

Supports Chrome v68-70

Changes include:
* Fixed ClickEelement in Mobile Emulation
* Fixed whitelisted IPs with IPv4
* Fixed starting ChromeDriver with whitelisted-ips flag on Mac OS
* Fixed SetTimeout to accept both pre-W3C and W3C formats
* Fixed take element screenshot
* Fixed ChromeDriver is looking for Chrome binaries in a system PATH as well
* Fixed Maximize window and Full Screen
* Implemented log-replay functionality. ( Does not work for Android and Remote Browser yet )
* Fixed some error codes were not compliant to W3C standard
* Fixed console.log with multiple arguments not handled properly
* Fixed GetElementRect should allow doubles
* Fixed touch emulation


### ChromeDriver 2.41

Supports Chrome v67-69

Changes include:
* Fixed issue when ChromeDriver runs with "whitelisted-ips" option
* Remote Debugging Port is returned in capabilities
* Implemented getting window size on Android
* Desktop Chrome launch error messages are improved
* ChromeDriver fails fast when unable to start Chrome binaries
* Close Window return value conforms with spec

## ChromeDriver 2.40

Supports Chrome v66-68

Changes include:
* Fixed Chromedriver hang on open when user-data-dir is specified and exists
* ChromeDriver supports IPv6 on requests
* Fixed Chromedriver couldn't find the Android file using valid file path
* /session/:sessionId/send_command and /session/:sessionId/send_command_and_get_result changed to proper extension commands