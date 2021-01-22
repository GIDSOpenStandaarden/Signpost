*If you need an introduction for this GitHub ‘GIDS Open Standaarden’ or more background information in Dutch, [click here](https://github.com/GIDSOpenStandaarden/Introduction).*

**Issues with components?** Please report those in the relevant repository. If you want guidance, please follow the good practice [shared by testlio here](https://testlio.com/blog/the-ideal-bug-report/). Alternatively, you can always contact us at info@gidsopenstandaarden.org. 

We distinguish between **five states** for open source components:

1. **R&D**: we are still researching, describing, and conceptualizing.
2. **POC**: Proof of Concept, a first implementation is being realized and tried out. Cannot be used in production settings.
3. **Beta**: the component is used in a few places.
4. **Production**: the component is used in many places.
5. **Abandoned**: we do not, or no longer maintain and/or support the component. Contact the developer directly if you want to obtain support, or contact us if you want to contribute and re-activate an open source component.  


# Overview of repositories

## SamenBeter Social Network Standard (SNS)
Currently, we share open source components to start third party applications (eHealth modules) from portals (SNS/Launch), and to identify users arriving in a module from a portal through such a launch using [IRMA](https://github.com/privacybydesign) (SNS/Identity). We are working on components to connect social networks to healthcare contexts, such as community portals or personal health record applications (SNS/Community). SNS/Launch, currently in use in [SamenBeter Proeftuinen](https://www.samenbeter.org/proeftuinen) and [Fitknip](https://www.samenbeter.org/fitknip) projects, will be succeeded in new implementations with GIDS Health Tools Interoperability (HTI), see below.

## GIDS Health Tools Interoperability (HTI)
HTI is an open standard that support the shared function to start third party applications anonymously. It is inspired by the proven international education open standard IMS-LTI and can be (re)used in different initiatives, like SamenBeter, MedMij, and Koppeltaal. It succeeds and replaces SNS/Launch, see above. Review [the proposal for HTI here](https://drive.google.com/open?id=1A89P3aHsSudeE2Iz2c3IVl30l9_USWrKb1SqYneJWKw).

### HTI | Production
- [GIDS-HTI-TestSuite](https://github.com/GIDSOpenStandaarden/GIDS-HTI-TestSuite). intended for developers to support the implementation of the HTI protocol.

### SNS/Identity: IRMA | POC
Within GIDS we use IRMA to authenticate and authorize users. IRMA is an open source privacy friendly way of identifying and authorizing, using attributes. It has been developed in the Netherlands by the Privacy by Design foundation. It is currently in use by the City council of Amsterdam and the Dutch government is considering IRMA as a solution for authentication alongside Digid. 

- [OpenSNS-IRMA-Auth](https://github.com/GIDSOpenStandaarden/OpenSNS-IRMA-Auth) tool to abstract implementation complexity away from other applications.
- [OpenSNS-IRMA-Docker](https://github.com/GIDSOpenStandaarden/OpenSNS-IRMA-Docker) contains the containerized deployment of an IRMA go server.

### SNS/Community: Solid | POC
Being able to store and share data is an important component within GIDS. Solid allows people to store their data securely in decentralized data stores called Pods. This is a secure personal web server that can store multiple types of data. The owner of the pod can control who and what can access that data. The data in the pod is accessible via the Solid Protocol. Solid is led by Sir Tim Berners Lee and is available as Open Source.
This service has been setup to prove that a portal and module application can store data using FHIR in a personal data store.
- No repositories yet, will be uploaded Q1 2021.
 
### SNS/Launch | Beta - Abandoned
We suggest current users to implement HTI, which succeeds the Launch-protocol.

- [OpenSNS-Launch-Protocol](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-Protocol) technical specification.
- [OpenSNS-Launch-Emulator](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-Emulator) test tool for consumer and producer.
- [OpenSNS-Launch-Java](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-Java) code example.
- [OpenSNS-Launch-PHP](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-PHP) code example.
- [OpenSNS-Launch-Python](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-Python) code example.
 
## Legal documents and templates
We host a few relevant legal components (governance, risk and compliance documentation) and templates that help you implement our licensing policies easily as you make use of, or contribute to our projects:

- [GIDSOpenStandaarden-LegalDocuments](https://github.com/GIDSOpenStandaarden/GIDSOpenStandaarden-LegalDocuments). [Beta] Repository of legal documents relevant for SNS and GIDS Open Standaarden.
- [GIDSOpenStandaarden-Templates](https://github.com/GIDSOpenStandaarden/GIDSOpenStandaarden-Templates). [Beta]. This repository contains templates that we use to organize GitHub GIDS Open Standaarden.
 
## MedMij implementation building components
We share open source components to help implement the functions required to [participate in MedMij](https://www.medmij.nl/open-source-bouwstenen/), a set of agreements to enable Dutch personal health record (PGO) applications (OpenPGO). Please take note that currently these components are not updated to the most recent version of MedMij.

If you want to use the components, please check them for compliance first, and if needed, update them to the latest MedMij version. Contact the developer directly if you want to obtain support, or contact us if you want to contribute. We are working to organize financial support to further develop and maintain these components.

### MedMij Implementation Building Blocks | Abandoned
- [OpenPGO-Medmij-ImplementatieBouwstenen-Opdracht](https://github.com/GIDSOpenStandaarden/OpenPGO-Medmij-ImplementatieBouwstenen-Opdracht). Assignment for the participants in the challenge to make the MedMij implementation building blocks
- [OpenPGO-Medmij-ImplementatieBouwstenen-Java](https://github.com/GIDSOpenStandaarden/OpenPGO-Medmij-ImplementatieBouwstenen-Java). Java implementation of the MedMij implementation building blocks.
- [OpenPGO-Medmij-ImplementatieBouwstenen-Dotnet](https://github.com/GIDSOpenStandaarden/OpenPGO-Medmij-ImplementatieBouwstenen-Dotnet) .NET implementation of the MedMij implementation building blocks.
- [OpenPGO-Medmij-ImplementatieBouwstenen-NodeJS](https://github.com/GIDSOpenStandaarden/OpenPGO-Medmij-ImplementatieBouwstenen-NodeJS) Node.js implementation of the MedMij implementation building blocks.
- [OpenPGO-Medmij-ImplementatieBouwstenen-PHP](https://github.com/GIDSOpenStandaarden/OpenPGO-Medmij-ImplementatieBouwstenen-PHP). PHP implementation of the MedMij implementation building blocks.
- [OpenPGO-Medmij-ImplementatieBouwstenen-Python](https://github.com/GIDSOpenStandaarden/OpenPGO-Medmij-ImplementatieBouwstenen-Python). Python implementation of the MedMij implementation building blocks.
- [OpenPGO-Medmij-ImplementatieBouwstenen-Python-OAuth](https://github.com/GIDSOpenStandaarden/OpenPGO-Medmij-ImplementatieBouwstenen-Python-OAuth) Python implementation of the MedMij OAuth Flow.
