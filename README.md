# Veracode-SBOM-WUI
Veracode SBOM generator with terminal based user interface for generting an SBOM from an Agent-based scan or application profile
This repo is a collection of SBOM Utilities that can be utilized from within the CLI to help generate SBOMs using Veracodes APIs

> Docker is currently needed in order to run this script (SBOM.sh, SBOM-GenV2.sh)    
> Python is required for the one that doesn't utilize docker containers     (SBOM-v1.sh , SBOM-Gen.sh)

In order to use this tool you have to have the following requirements:
- Docker installed on the machine or [Httpie](https://docs.veracode.com/r/c_httpie_tool) and the [Python Authentication Library](https://docs.veracode.com/r/t_install_api_authen) 
- a credentials file stored on the machine in the proper location: https://docs.veracode.com/r/t_configure_credentials_mac
- a workspace project or application profile that you would like to generate an SBOM for


### Design choices ###

The menu function used is the script can be found [here](https://unix.stackexchange.com/questions/146570/arrow-key-enter-menu) using the cursor blinker for selection
It was between the dialog option and the native keyboard escape option. I chose to utilize the native keyboard escape function since it wouldn't require anything to be installed.


### Find a Bug, Report a Bug ###

If you see a bug, please create an issue or leave a comment
If you are able to fix a bug, please create a pull request and then reference the issue for review
