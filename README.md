# Team Contrib

This repository is intended to make the process of reviewing teammates code less error-prone, 
using automated tools to check and help to correct common mistakes.

Based on this [blog post](http://tech.zumba.com/2014/04/14/control-code-quality/) by Chris Saylor.

## Git Hook
An pre-commit hook is provided on the install of the project.
All is needed is to execute an

    composer install

## PHP Lint
The lint tool checks for script errors, so the php parser itself is used.

## PHP Code Sniffer
The Code Sniffer and the Code Beautifier tools are used to ensure the code quality based on the standards defined.
The PSR2 are the default set, but any standards can be applied.

To change the standards, modify the file **contrib/phpcs/teamcontrib.xml**

Code Beautifier is executed first to correct small mistakes as indentation, spaces, and other formatting errors.

Code Sniffer tool is used to check for common mistakes that make the code still don't adhere to the standards.

## PHP Mess Detector
The code is verified against the PHPMD rule sets, ensuring that certain code standards are followed.

To change the rules applied, modify the file **contrib/phpmd/teamcontrib.xml**

More about the PHPMD and the rule sets applied, [here](http://phpmd.org/).
