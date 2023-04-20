NUnit HTML Report Generator
===========================
This project is used to convert NUnit (V2) generated XML result files into a self-contained Bootstrap 3 based HTML page. The page is designed to be responsive and viewable on mobile and desktop devices. It has been tested on Windows 8 under Chrome and IE and Chrome for Android.

##Latest Update
* We've made updates to support processing of multiple XML files at once, along with the ability to generate a summary file that includes overall statistics and links to individual files. This feature makes it easier to view all the results in one place and also allows for easy navigation to specific files.
* Upgraded to .Net Framework Version 4.8

##Example
* [Click here to view the example output](http://htmlpreview.github.io/?https://github.com/JatechUK/NUnit-HTML-Report-Generator/blob/master/ExampleResults.html)
* [Click here to see the input that generated the output](https://raw.githubusercontent.com/JatechUK/NUnit-HTML-Report-Generator/master/NUnit%20HTML%20Report%20Generator/ExampleResults.xml)

##Building 
1. Open in Visual Studio 2022
2. Click Build > Build Solution

##Running in Visual Studio

Included in the project is an example NUnit XML results file originally found at [vincentp-tests playground](https://github.com/vincentp-test/playground/blob/master/test-results.xml). The project has a debug command line arguement set in the project settings that will pass the filename of the example file into the software to generate a HTML file. Clicking the Start Debugging/F5 button in visual studio will run the software and generate a HTML file based on the example XML file. The output file will be found in the same directory as your executable (bin).

##Standard Usage

Download the latest release from the [releases page](https://github.com/JatechUK/NUnit-HTML-Report-Generator/releases) and extract the files onto your machine. The application can be called from the command line as follows: 

`NUnitHTMLReportGenerator.exe [input-file-path] [output-file-path]` -- to convert single XML file into HTML

`NUnitHTMLReportGenerator.exe [input-folder-path] [output-folder-path]` -- to convert multiple XML files just tell the input folder path only and output folder path and it will generate all the HTML files + one summary file named 'NUnitTestsSummary.html' in the output folder.

##Disclaimer
This project is maintained by [Luke Browning](http://github.com/luke-browning) on behalf of [Jatech](http://github.com/JatechUK) and is released under the [GPLv2.0](https://raw.githubusercontent.com/JatechUK/NUnit-HTML-Report-Generator/master/LICENSE).
