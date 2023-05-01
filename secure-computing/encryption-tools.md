
# Encryption tools

Here you can find a list of encryption tools. There are many more encryption tools and packages available - here we selected the ones most commonly used. If you want to know more, there is a very extensive [comparison of encryption software](https://en.wikipedia.org/wiki/Comparison_of_disk_encryption_software) on Wikipedia.

### Important notes 
- When encrypting data, it is always important to store the key to decrypt the data in a safe location such as a password manager. It is often the case that once you lose the key, you lose access to the data. 
- When sharing encrypted data with others, make sure you share the password or decryption key via another way than how you share the data.
- Some encryption tools can use keyfiles besides passwords that are needed to decrypt the data. These can either be created by the tool, or you can use personal files like a specific picture.

## Full drive encryption

The tools in the table below can be used to encrypt an entire drive. This is useful to protect data on personal devices or external disks like USB sticks.

| Name | Description | Technique | More info | Maintenance | GitHub stars | License |
| --- | --- | --- | --- | --- | --- | --- |
| [Veracrypt](https://www.veracrypt.fr/en/Home.html) | [Open source](https://sourceforge.net/projects/veracrypt/files/) file and drive encryption software for Windows, Mac OS and Linux. | AES-256, Serpent, Twofish, etc. | [Documentation](https://www.veracrypt.fr/en/Documentation.html), [FAQ](https://www.veracrypt.fr/en/FAQ.html), [Beginner's tutorial](https://www.veracrypt.fr/en/Beginner%27s%20Tutorial.html) | Active | NA | [Apache 2.0 and Truecrypt 3.0](https://sourceforge.net/p/veracrypt/code/ci/master/tree/License.txt) |
| [Bitlocker](https://learn.microsoft.com/en-us/windows/security/information-protection/bitlocker/bitlocker-overview) | Drive encryption software built into Windows. | XTS-AES with 128-bit or 256-bit keys | [Documentation](https://learn.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2008-R2-and-2008/cc731549(v=ws.10)), [FAQ](https://learn.microsoft.com/en-us/previous-versions/windows/it-pro/windows-vista/cc766200(v=ws.10)), [set up on Windows](http://www.howtogeek.com/192894/how-to-set-up-bitlocker-encryption-on-windows/) | Inactive | NA | Unknown |
| FileVault2 | Built-in encryption software for MacOS to encrypt the entire startup volume. | XTS-AES-128 with a 256 bit key | [Manual](https://support.apple.com/en-us/HT204837) | Active | NA | Unknown |  
| [GnuPG2](https://gnupg.org/index.html) | Free encryption software for Windows, Linux and MacOS to encrypt messages, files, folders and drives. | AES-128, AES-256, 3DES, Blowfish, RSA, [etc.](https://en.wikipedia.org/wiki/GNU_Privacy_Guard#Algorithms) | [Guides](https://gnupg.org/documentation/guides.html), [FAQ](https://gnupg.org/faq/gnupg-faq.html#oses) [Front-ends](https://gnupg.org/software/frontends.html)| Active | NA | GPL-v3 |
| [dm-crypt](https://gitlab.com/cryptsetup/cryptsetup) | [Open source](https://gitlab.com/cryptsetup/cryptsetup) command-line software for drive encryption on Linux | AES, Twofish, Serpent | [wiki](https://gitlab.com/cryptsetup/cryptsetup/-/wikis/DMCrypt) | Active | 500-1000 | [LGPL](https://gitlab.com/cryptsetup/cryptsetup/-/blob/main/COPYING.LGPL) |  


## File- and folder encryption
The tools in the table below describe tools that can encrypt files and folders locally. Note that there are also tools that do not have encryption as their primary purpose, but as an additional functionality, such as [Microsoft Office](https://support.microsoft.com/en-us/windows/how-to-encrypt-a-file-1131805c-47b8-2e3e-a705-807e13c10da7), [LibreOffice](https://help.libreoffice.org/6.3/en-US/text/shared/guide/protection.html) and [SPSS](https://www.ibm.com/support/pages/can-you-password-protect-ibm-spss-file).

| Name | Description | Technique | More info | Maintenance | GitHub stars | License |
| --- | --- | --- | --- | --- | --- | --- | 
| [Cryptomator](https://cryptomator.org) | [Open source](https://github.com/cryptomator/cryptomator) tool to encrypt files, folders and file names. Suitable for Windows, Linux, mac OS, Android and iOS and optimized for cloud storage | AES-256 | [Documentation](https://docs.cryptomator.org/en/latest/), [community forum](https://community.cryptomator.org/) | Active | 1000+ | [GPL-v3](https://github.com/cryptomator/cryptomator/blob/develop/LICENSE.txt) |
| [Veracrypt](https://www.veracrypt.fr/en/Home.html) | [Open source](https://sourceforge.net/projects/veracrypt/files/) file and drive encryption software for Windows, Mac OS and Linux. | AES-256, Serpent, Twofish, etc. | [Documentation](https://www.veracrypt.fr/en/Documentation.html), [FAQ](https://www.veracrypt.fr/en/FAQ.html), [Beginner's tutorial](https://www.veracrypt.fr/en/Beginner%27s%20Tutorial.html) | Active | NA | Unknown |
| [Boxcryptor](https://www.boxcryptor.com/en/) | Encryption of files and folders stored at cloud providers like OneDrive, Google Drive, etc. for Windows, Mac, Android, iOS, and Microsoft Teams. | End-to-end, AES-256, RSA-4096 | [Help pages](https://support.boxcryptor.com/en/help/overview/windows/) | Active | NA | Unknown |
| [AES Crypt](https://www.aescrypt.com/download/) | [Open source](https://www.aescrypt.com/download/#gitrepos) software for encrypting files and folders in Windows, MacOS, Linux, iOS and Android | AES-256 | [Documentation](https://www.aescrypt.com/documentation/) | Active | NA | Unknown |
| [7-Zip](https://www.7-zip.org/) | Compression software for Windows. | AES-256 | [7-Zip FAQs](https://www.7-zip.org/faq.html), [how to for MacOS and Linux](http://www.howtogeek.com/203590/how-to-create-secure-encrypted-zip-or-7z-archives-on-any-operating-system/), [how to for Windows](https://geo-data-support.sites.uu.nl/manuals/7-zip/file-encryption-7zip/) | Active | NA | [GNU LGPL and BSD-3 Clause](https://www.7-zip.org/license.txt) |
| [AxCrypt](https://www.axcrypt.net/) | Open source encryption tool for Windows, Mac OS, Linux, iOS, Android. | AES-128, AES-256 | [Get started](https://www.axcrypt.net/information/guides/get-started/), [FAQ](https://www.axcrypt.net/information/faq/), [forums](https://forum.axcrypt.net/forums/) | Active | NA | Free version: [GPL-v3](https://www.axcrypt.net/information/terms-of-use/)  |
| [GnuPG2](https://gnupg.org/index.html) | Free encryption software for Windows, Linux and MacOS to encrypt messages, files and folders. | AES-128, AES-256, 3DES, Blowfish, RSA, [etc.](https://en.wikipedia.org/wiki/GNU_Privacy_Guard#Algorithms) | [Guides](https://gnupg.org/documentation/guides.html), [FAQ](https://gnupg.org/faq/gnupg-faq.html#oses), [Front-ends](https://gnupg.org/software/frontends.html) | Active | NA | GPL-v3 |
| [EncFS](https://vgough.github.io/encfs/) | [Open source](https://github.com/vgough/encfs) command-line-based software for Linux and Mac OS. | AES, Blowfish, etc. | [Manual](https://github.com/vgough/encfs/blob/master/encfs/encfs.pod) | Inactive | 1000+ | [LGPL](https://github.com/vgough/encfs/blob/master/COPYING.LGPL) |

