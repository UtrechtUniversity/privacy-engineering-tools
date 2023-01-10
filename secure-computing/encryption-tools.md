# Encryption tools

Here you can find a list of encryption tools. Please note that this is Work In Progress. Any suggestions for improvement are welcome.

**Important notes**  
- When encrypting data, it is always important to store the key to decrypt the data in a safe location such as a password manager. It is often the case that once you lose the key, you lose access to the data. 
- When sharing encrypted data with others, make sure you share the password or decryption key via another way than how you share the data.
- Some encryption tools can use keyfiles besides passwords that are needed to decrypt the data. These can either be created by the tool, or you can use personal files like a specific picture.

## Full drive encryption

The tools in the table below can be used to encrypt an entire drive. This is useful to protect data on personal devices or external disks like USB sticks.

| Name | Description | Technique | More info | Maintenance | GitHub stars | License |
| --- | --- | --- | --- | --- | --- | --- |
| [Veracrypt](https://www.veracrypt.fr/en/Home.html) | [Open source](https://sourceforge.net/projects/veracrypt/files/) file and drive encryption software for Windows, Mac OS and Linux. The encrypted folder or drive can be mounted to file exporer for actively working on data. Can also use keyfiles. | AES-256, Serpent, Twofish, AES-Serpent, AES-Twofish- Serpent, etc. | [Documentation](https://www.veracrypt.fr/en/Documentation.html), [FAQ](https://www.veracrypt.fr/en/FAQ.html), [Beginner's tutorial](https://www.veracrypt.fr/en/Beginner%27s%20Tutorial.html) | Active | NA | Unknown |
| [Bitlocker](https://learn.microsoft.com/en-us/windows/security/information-protection/bitlocker/bitlocker-overview) | Drive encryption software for Windows, requires a [Trusted Platform Module](https://www.howtogeek.com/287737/how-to-check-if-your-computer-has-a-trusted-platform-module-tpm-chip/) in the to-be-encrypted device. | AES-256 | [Documentation](https://learn.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2008-R2-and-2008/cc731549(v=ws.10)), [FAQ](https://learn.microsoft.com/en-us/previous-versions/windows/it-pro/windows-vista/cc766200(v=ws.10)), [set up on Windows](http://www.howtogeek.com/192894/how-to-set-up-bitlocker-encryption-on-windows/) | Inactive | NA | Unknown |
| FileVault2 | Encryption software for MacOS | ... | [Manual](https://support.apple.com/en-us/HT204837) | ... | ... | ... |  
| dm-crypt | Encryption functionality for Linux | ... | ... | ... | ... | ... | ... | 

## File- and folder encryption
The tools in the table below describe tools that can encrypt files and folders locally. Note that there are also tools in this list that do not have encryption as their primary purpose, but as an additional functionality. 

| Name | Description | Technique | More info | Maintenance | GitHub stars | License |
| --- | --- | --- | --- | --- | --- | --- | 
| [Cryptomator](https://cryptomator.org) | [Open source](https://github.com/cryptomator/cryptomator) tool to encrypt files, folders and file names in a vault that is temporarily mounted to file explorer when unlocked. Possibility for offline key recovery, detection of sync conflicts. Suitable for Windows, Linux, maxOS, Android and iOS and optimized for cloud storage | AES-256 | [Documentation](https://docs.cryptomator.org/en/latest/), [community forum](https://community.cryptomator.org/) | Active | 1000+ | [GPL-v3](https://github.com/cryptomator/cryptomator/blob/develop/LICENSE.txt) |
| [Veracrypt](https://www.veracrypt.fr/en/Home.html) | [Open source](https://sourceforge.net/projects/veracrypt/files/) file and drive encryption software for Windows, Mac OS and Linux. The encrypted folder or drive can be mounted to file exporer for actively working on data. Can also use keyfiles. | AES-256, Serpent, Twofish, AES-Serpent, AES-Twofish- Serpent, etc. | [Documentation](https://www.veracrypt.fr/en/Documentation.html), [FAQ](https://www.veracrypt.fr/en/FAQ.html), [Beginner's tutorial](https://www.veracrypt.fr/en/Beginner%27s%20Tutorial.html) | Active | NA | Unknown |
| [Boxcryptor](https://www.boxcryptor.com/en/) | Encryption of files and folders stored at cloud providers like OneDrive, Google Drive, etc. for Windows, Mac, Android, iOS, and Microsoft Teams. Allows file access sharing | End-to-end, AES-256, RSA-4096 | [Help pages](https://support.boxcryptor.com/en/help/overview/windows/) | Active | NA | Unknown |
| [AES Crypt](https://www.aescrypt.com/download/) | [Open source](https://www.aescrypt.com/download/#gitrepos) software for encrypting files and folders in Windows, MacOS, Linux, iOS and Android | AES-256 | [Documentation](https://www.aescrypt.com/documentation/) | Active | NA | Unknown |
| [7-Zip](https://www.7-zip.org/) | Compression software for Windws that can also encrypt a zipped folder | AES-256 | [7-Zip FAQs](https://www.7-zip.org/faq.html), [how to for MacOS and Linux](http://www.howtogeek.com/203590/how-to-create-secure-encrypted-zip-or-7z-archives-on-any-operating-system/) | Active | NA | [GNU LGPL and BSD-3 Clause](https://www.7-zip.org/license.txt) |
| SPSS | Statistical analysis software that can encrypt files with a password at saving | ... | ... | ... | ... | ... |
| Office | Both Microsoft and Libre office have encryption functionality to encrypt individual files with a password: File > Protect workbook/document > Encrypt with password |  ... | ... | ... | ... | ... |

## TODO
| Name | Description | Technique | More info | Maintenance | GitHub stars | License |
| --- | --- | --- | --- | --- | --- | --- |
| GnuPG2 | Open source encryption tool for Windows, Linux and MacOS, messaging | AES-128, AES-256, 3DES | ... | ... | ... |
| openssl | Toolkit for symmetric encryption | AES-256 | ... | ... | ... | ... |

Complete:
- Filevault2
- dm-crypt
- SPSS
- Office

Also look at: https://en.wikipedia.org/wiki/Comparison_of_disk_encryption_software