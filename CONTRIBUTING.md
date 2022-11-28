# Contributing

**When submitting a bug report, please follow this guidelines.**

Operating System: 

Current Elpis Version: 

Using proxy/vpn:

Steps to reproduce the problem:

Problem: 

# Creating a release

1. Update the version number in AssemblyInfo.cs
2. Update the ChangeLog.txt
3. Build the solution (AppRelease config - make sure to include a valid ReleaseData.cs file in the Elpis project)
4. Build the ElpisSetup project
5. Zip the contents of <solution>/Elpis/bin/AppRelease (`Elpis_portable_<version>.zip`), include this in the release.
6. Open a command prompt in the ElpisSetup dir
7. Run `iexpress`
8. "Open existing Self Extraction Directive file:" -> Navigate to the .SED file in the ElpisSetup dir.
9. Click through the rest of the prompts to make the self-extracting archive.
10. Include <solution>/ElpisSetup/Install/ElpisInstall.exe (rename to include version number: `ElpisInstall_<version>.exe`) in the release.
