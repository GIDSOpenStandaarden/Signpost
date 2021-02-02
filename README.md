*If you need an introduction for this GitHub ‘GIDS Open Standaarden’ or more background information in Dutch, [click here](https://github.com/GIDSOpenStandaarden/Introduction).*

**Issues with components?** Please report those in the relevant repository and use "@name"to assign a member. If you want guidance, please follow the good practice [shared by testlio here](https://testlio.com/blog/the-ideal-bug-report/). Alternatively, you can always contact us at info@gidsopenstandaarden.org. 

We distinguish between **five states** for open source components:

1. **R&D**: we are still researching, describing, and conceptualizing.
2. **POC**: Proof of Concept, a first implementation is being realized and tried out.
3. **Beta**: the component is used in a few places.
4. **Production**: the component is used in many places.
5. **Abandoned**: we do not, or no longer maintain and/or support the component. Contact the developer directly if you want to obtain support, or contact us if you want to contribute and re-activate an open source component.  


# Overview of repositories

## GIDS Health Tools Interoperability (HTI)
HTI is an open standard that support the shared function to start third party applications. It is inspired by the proven international education open standard IMS-LTI and can be (re)used in different initiatives, like Beter met Elkaar projects (SamenBeter Proeftuin Wijken en FitKnip Duurzame Financiering), MedMij, and Koppeltaal. It succeeds and replaces SNS/Launch, see below. 

### HTI | POC
- [GIDS-HTI-Protocol](https://github.com/GIDSOpenStandaarden/GIDS-HTI-Protocol) technical specification.
- [GIDS-HTI-TestSuite](https://github.com/GIDSOpenStandaarden/GIDS-HTI-TestSuite) intended for developers to support the implementation of the HTI protocol.
- [GIDS-HTI-RI-Module-Python](https://github.com/GIDSOpenStandaarden/GIDS-HTI-RI-Module-Python) code example.
- [GIDS-HTI-RI-Module-Java](https://github.com/GIDSOpenStandaarden/GIDS-HTI-RI-Module-Java) code example.
- [GIDS-HTI-RI-Portal-Java](https://github.com/GIDSOpenStandaarden/GIDS-HTI-RI-Portal-Java) code example.

## Social Network Standard (SNS)
Currently, we share open source components to start third party applications (eHealth modules) from portals (SNS/Launch), and to identify users arriving in a module from a portal through such a launch using [IRMA](https://github.com/privacybydesign) (SNS/Identity). We are working on components to connect social networks to healthcare contexts, such as community portals or personal health record applications (SNS/Community). SNS/Launch, currently in use in Stichting Beter met Elkaar projects; [SamenBeter Proeftuin Wijken](https://www.samenbeter.org/proeftuinen) and [FitKnip Duurzame Financiering](https://www.samenbeter.org/fitknip), will be succeeded in new implementations with GIDS Health Tools Interoperability (HTI), see above.

### SNS/Launch | Beta
- [OpenSNS-Launch-Protocol](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-Protocol) technical specification.
- [OpenSNS-Launch-Emulator](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-Emulator) test tool for consumer and producer.
- [OpenSNS-Launch-Java](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-Java) code example.
- [OpenSNS-Launch-PHP](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-PHP) code example.
- [OpenSNS-Launch-Python](https://github.com/GIDSOpenStandaarden/OpenSNS-Launch-Python) code example.

### SNS/Identity | POC
- [OpenSNS-IRMA-Auth](https://github.com/GIDSOpenStandaarden/OpenSNS-IRMA-Auth) tool to abstract implementation complexity away from other applications.
- [OpenSNS-IRMA-Docker](https://github.com/GIDSOpenStandaarden/OpenSNS-IRMA-Docker) contains the containerized deployment of an IRMA go server.

### SNS/Community | R&D
- No repositories yet.
 
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
