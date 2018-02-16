# ansible-hana-studio
This Skript runs the installation of HANA studio on Fedora and RHEL.
If you want to add architectures, please commit your code to this repository

## Prerequisites

To install HANA Studio on your Linux platform you need to download the following software packages

 . SAP HANA Client for your platform
 . SAP HANA Studio for your platform
 . SAPCAR to unpack the software

You will find the packages at https://support.sap.com/swdc. 
 - Click on *Access downloads* at *Support Packages & Patches*
 - Click on *H* for SAP HANA etc.
 - Click on *SAP HANA Platform Edition 2.0*
 - Click on *SAP HANA CLIENT 2.0*
 - Add *IMDB_CLIENT*.SAR* for your SAP HANA release to the download basket, e.g. IMDB_CLIENT20_002_36-80002082.SAR for SAP HANA 2 SPS 02 to the download basket 
 - go Back
 - Click on *SAP HANA PLATFORM EDITION 2.0* in the breadcrump path at the top of the page to go back one level
 - Click on *SAP HANA STUDIO 2*
 - Add *IMC_STUDIO2_*.SAR* for your SAP HANA release to the download basket, e.g. IMC_STUDIO2_220_0-80000321.SAR
 - In the searchbar enter SAPCAR and add the latest version for Linux x86_64 to the downlaod basket
 - Download these components and make them accessible on the client, where you want to install HANA studio

## Define variables in the playbook
[%hardbreaks]
sapcar: path to sapcar executable
hana_client: path to previous downloaded SAP HANA Client
hana_studio: path to previous downloaded SAP HANA Studio package


