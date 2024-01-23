# MUSAP Project
MUSAP: "Multiple SSCD with Unified Signature API Library" aims to develop a new software interface called Unified Signature Application Programming Interface (USAPI) Library.
MUSAP will act as an intermediary layer that abstracts the complexities of different SSCD technologies and provides a unified API Library for developers. 
The primary objective of the MUSAP project has been three fold: 
    1. To develop an open-source API library that streamlines the integration of various Secure Signature Creation Devices (SSCDs) into smartphone applications, thereby facilitating the creation of robust authentication and signature solutions. 
    2. MUSAP aims to seamlessly integrate with both centralized and decentralized identity management systems, allowing SSCD keys to function effectively in both environments. This approach empowers end-users to access services without being constrained by the specific identity management model in use. 
    3. To allow support for multiple certificates/credentials in one device. This approach demonstrates MUSAP’s user-centric approach, where giving option to choose which SSCD they want to have their private keys in, and allows end-users to have identities with various level of assurances in use.


## MUSAP Repositories 
Methics has developed MUSAP libraries and reference apps for demonstration and pilots. Following software code is developed so far:
1.	MUSAP API Specification: Informative repository documenting MUSAP specifications
2.	[MUSAP Android Library](https://github.com/methics/musap-android): Repository about MUSAP Android library 
3.	[MUSAP iOS Library](https://github.com/methics/musap-ios): Repository about MUSAP iOS library
4.	[MUSAP Link Library (java) ](https://github.com/methics/musap-link): Repository about component of MUSAP deployed on backend (server)
5.	[Android Reference app for MUSAP ](https://github.com/methics/musap-demo-android): Reference Demo app for Android using MUSAP Android Library 
6.	[iOS Reference app for MUSAP ](https://github.com/methics/MUSAP-Demo-App-iOS):  Reference Demo app for iOS using MUSAP iOS Library


## APIS in MUSAP
Overall MUSAP project will provide three distinct APIs: 
1.	MUSAP API (Native Android or iOS)
2.	MUSAP Link API (REST): API for Relying Parties to request signature through MUSAP
3.	MUSAP Coupling API (JSON): To link MUSAP Library and MUSAP Link
Image below illustrates MUSAP scope, which highlights all above-mentioned APIs. 



