*If you need an introduction for this GitHub ‘GIDS Open Standaarden’ or more background information in Dutch, [click here](https://github.com/GIDSOpenStandaarden/Introduction).*

**Issues with components?** Please report those in the relevant repository and use "@name"to assign a member. If you want guidance, please follow the good practice [shared by testlio here](https://testlio.com/blog/the-ideal-bug-report/). Alternatively, you can always contact us at info@gidsopenstandaarden.org. 

We distinguish between **five states** for open source components:

1. **R&D**: we are still researching, describing, and conceptualizing.
2. **POC**: Proof of Concept, a first implementation is being realized and tried out. Cannot be used in production settings.
3. **Beta**: the component is used in a few places.
4. **Production**: the component is used in many places.
5. **Abandoned**: we do not, or no longer maintain and/or support the component. Contact the developer directly if you want to obtain support, or contact us if you want to contribute and re-activate an open source component.  


# Overview of repositories (newest to oldest)
## GIDS Health Tools Interoperability (HTI) 
HTI is an open standard that supports the shared function to anonymously start/launch from a portal to a third party application(s). It is inspired by the proven international education open standard IMS-[LTI](https://www.imsglobal.org/activity/learning-tools-interoperability) and can be (re)used in different initiatives, like [Beter met Elkaar](https://www.betermetelkaar.org/), [MedMij](https://www.medmij.nl/), and [Koppeltaal](https://www.koppeltaal.nl/). It succeeds and replaces SNS/Launch, see above.  It has been developed by [Headease](https://www.headease.nl/) within the project [Samenbeter](https://www.samenbeter.org/) from the [foundation Beter Met Elkaar](https://www.betermetelkaar.org/).
 View [the protocol for HTI here](https://github.com/GIDSOpenStandaarden/GIDS-HTI-Protocol).

### HTI | Production
- [GIDS-HTI-Protocol](https://github.com/GIDSOpenStandaarden/GIDS-HTI-Protocol). Intended for developers to implement the protocol.
- [GIDS-HTI-TestSuite](https://github.com/GIDSOpenStandaarden/GIDS-HTI-TestSuite). intended for developers to support the implementation of the HTI protocol.
- [GIDS-HTI-RI-Module-Python](https://github.com/GIDSOpenStandaarden/GIDS-HTI-RI-Module-Python) code example.
- [GIDS-HTI-RI-Module-Java](https://github.com/GIDSOpenStandaarden/GIDS-HTI-RI-Module-Java) code example.

## SamenBeter Social Network Standard (SNS)
Currently, we develop SNS in 3 phases of open source components to start third party applications (eHealth modules) from portals (1. SNS/Launch - replaced by HTI), and to identify users arriving in a module from a portal through such a launch using [IRMA](https://github.com/privacybydesign) (2. SNS/Identity). We are working on components to connect social networks to healthcare contexts, such as community portals or personal health record applications (3. SNS/Community). SNS/Launch, currently in use in Stichting Beter met Elkaar projects; [SamenBeter Proeftuin Wijken](https://www.samenbeter.org/proeftuinen) and [FitKnip Duurzame Financiering](https://www.samenbeter.org/fitknip), will be succeeded in new implementations with GIDS Health Tools Interoperability (HTI), see above.

### SNS/Identity: IRMA | POC
Within GIDS we use IRMA to authenticate and authorize users, for example when they arrive in a third party application via HTI or when accessing their Solid Pod. IRMA is an open source privacy friendly way of identifying and authorizing, using attributes. It has been developed in the Netherlands by the Privacy by Design foundation. It is currently in use by the City council of Amsterdam and the Dutch government is considering IRMA as a solution for authentication alongside Digid. 

- [OpenSNS-IRMA-Auth](https://github.com/GIDSOpenStandaarden/OpenSNS-IRMA-Auth) This service has been set up to easily experiment with IRMA for parties within SamenBeter or with an interest in using IRMA. It abstracts implementation complexity away from other applications.
- [OpenSNS-IRMA-Docker](https://github.com/GIDSOpenStandaarden/OpenSNS-IRMA-Docker) contains the containerized deployment of an IRMA go server.

### SNS/Community: Solid | POC
Being able to store and share data is an important component within GIDS. Solid allows people to store their data securely in decentralized data stores called Pods. This is a secure personal web server that can store multiple types of data. The owner of the pod can control who and what can access that data. The data in the pod is accessible via the [Solid Protocol](https://solid.github.io/specification/). Solid is led by Sir Tim Berners Lee and is available as Open Source.
This service has been setup to prove that a portal and module application can store data using FHIR in a personal data store.
- No Solid repositories yet, will be uploaded Q1 2021. The repo that will be made available has been set up to prove that a portal and module application can store data using FHIR in a personal data store.
- [GIDS-SNS-RI-Portal-Java](https://github.com/GIDSOpenStandaarden/GIDS-SNS-RI-Portal-Java) - Reference implementation of a portal to:
  - List e-health tasks and use HTI to anonymously launch these tasks. 
  - Connect to a Solid POD
  - Give read / write access to Solid POD

 
### SNS/Launch | Beta - Abandoned
We suggest current users to implement HTI, which succeeds the Launch-protocol.

- [OpenSNS-Launch-Protocol](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-Protocol) technical specification.
- [OpenSNS-Launch-Emulator](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-Emulator) test tool for consumer and producer.
- [OpenSNS-Launch-Java](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-Java) code example.
- [OpenSNS-Launch-PHP](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-PHP) code example.
- [OpenSNS-Launch-Python](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-Python) code example.
 
## Security, Legal documents and templates
Frameworks that help you implement policies easily for governance, risk and compliance. As you make use of, or contribute to our GIDS Open Standaarden open source components.

- [GIDSOpenStandaarden-SecurityFramework](https://github.com/GIDSOpenStandaarden/GIDSOpenStandaarden-SecurityFramework). [Beta] instructions for peer review or external audit.
- [GIDSOpenStandaarden-LegalDocuments](https://github.com/GIDSOpenStandaarden/GIDSOpenStandaarden-LegalDocuments). [Beta] legal commons, licences, processing agreement.
- [GIDSOpenStandaarden-Templates](https://github.com/GIDSOpenStandaarden/GIDSOpenStandaarden-Templates). [Beta]. template naming repositories. 
 
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
