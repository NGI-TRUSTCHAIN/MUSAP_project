# MUSAP Project

"MUSAP: "Multiple SSCD with Unified Signature API Library" aims to develop a new software interface called Unified Signature Application Programming Interface (USAPI) Library. MUSAP will act as an intermediary layer that abstracts the complexities of different SSCD technologies and provides a unified API Library for developers. 
The primary objective of the MUSAP project has been three fold: 
1. To develop an open-source API library that streamlines the integration of various Secure Signature Creation Devices (SSCDs) into smartphone applications, thereby facilitating the creation of robust authentication and signature solutions. 
2. MUSAP aims to seamlessly integrate with both centralized and decentralized identity management systems, allowing SSCD keys to function effectively in both environments. This approach empowers end-users to access services without being constrained by the specific identity management model in use. 
3. To allow support for multiple certificates/credentials in one device. This approach demonstrates MUSAP’s user-centric approach, where giving option to choose which SSCD they want to have their private keys in, and allows end-users to have identities with various level of assurances in use."


## MUSAP Repositories 
Following software code is developed so far:
1.	[MUSAP API Specification]: Informative repository documenting MUSAP API specifications
2.	[MUSAP Android Library](https://github.com/methics/musap-android): Repository about MUSAP Android library 
3.	[MUSAP iOS Library](https://github.com/methics/musap-ios): Repository about MUSAP iOS library
4.	[MUSAP Link Library (java) ](https://github.com/methics/musap-link): Repository about component of MUSAP deployed on backend (server)
5.	[Android Reference app for MUSAP ](https://github.com/methics/musap-demo-android): Reference Demo app for Android using MUSAP Android Library 
6.	[iOS Reference app for MUSAP ](https://github.com/methics/MUSAP-Demo-App-iOS):  Reference Demo app for iOS using MUSAP iOS Library
7.	[Divvy app for Client-DIDs project (Danubetech)]:Divvy app for Danubetech demo using MUSAP Android Library
8.	[VSign Android App API]: Sign App for vsign.mn Pilot using MUSAP Android Library to call Unitel mPKI SIM and GSign App 

Image below provides high level overview of MUSAP architecture.
![MUSAP project architecture](Picture1_MUSAP_D3_Architecture.png)


During OC1 of NGI Trustchain project, 4 key stores will be enabled for the end-user with MUSAP, i.e TEE (Android Key store or iOS Secure Enclave), eUICC/UCICC (Mobile ID), Dongle (Yubikey via NFC) and eIDAS Remote Signing.  As EDIW progressed, ENISA (European Cybersecurity Agency) has been releasing recommendations related to a need for harmonized interface that allows access to cryptographic operations. Image below incorporates MUSAP scope to act as a secure component API to enable SSCD for end-user. 
![MUSAP adapted picture from Enisa](Picture2_MUSAP_scope_ENISA_adaption.png)

MUSAP Library (Java/Swift) can be integrated with any Android or iOS app projects. Whereas, MUSAP Link Library (Servlet component) is delivered as a library that can be used with a Java-based web server.

Overall MUSAP project will provide three distinct APIs: 
1. MUSAP API (Native Android or iOS)
2. MUSAP Link API (REST): API for Relying Parties to request signature through MUSAP
3. MUSAP Coupling API (JSON): To link MUSAP Library and MUSAP Link

   
Image below illustrates MUSAP scope, which highlights all above-mentioned APIs. 

![MUSAP project APIs](Picture3_MUSAP_APIs.png)

## MUSAP Functionalities:
MUSAP has 10 defined functionalities (as mentioned in D1 and D2). These functionalities are listed below:
1. F1 i.e., Functionality 1 Integration of multiple SSCDs into MUSAP library
2. F2 i.e., Functionality 2 Open Interface for integrating new & multiple SSCDs with APP
3. F3 i.e., Functionality 3 Digital Signatures with different LoAs (High, Substantial)
4. F4 i.e., Functionality 4 Key discovery
5. F5 i.e., Functionality 5: Key lifecycle management (do defined key operations)
6. F6 i.e., Functionality 6: Key Attestation
7. F7 i.e., Functionality 7: Key metadata definition and import/export
8. F8 i.e., Functionality 8: Sign data and cryptographic formats
9. F9 i.e., Functionality 9: MUSAP Link library (Servlet component)
10. F10 i.e., Functionality 10: URI Scheme



## MUSAP Use Cases
Overall MUSAP project will provide three distinct APIs: 
1. Enable Type 1 (High) and Type 2 (Substantial) configurations of EUDIW in one device
2.	Sign any data format (X.509, VC, DID, etc.)
3.	Provide multiple keystores/sscds to end-user to sign/auth
4.	Handling Key Management methods and operations

MUSAP fact sheet can be found here: [MUSAP fact sheet](https://www.methics.fi/wp-content/uploads/2023/11/MUSAP_Product_Fact_Sheet.pdf)

Image below illustrates MUSAP uaw case for EUDIW 
![MUSAP for EUDIW](Picture4_MUSAP_for_EUDIW.png)


## About MUSAP and Methics
MUSAP Project has received funding from the NGI TrustChain project. Project is funded under the NGI initiative by the European Union (GA No 101093274). MUSAP will be released as an Open-Source Library in Github (TRL7 or higher) by April 2024. 

Methics is a Finnish technology vendor specializing in Digital Identity and Mobile Signatures services. Methics specializes in delivering standards based identity solutions. 
For more info visit [MUSAP website](https://methics.fi/musap)
