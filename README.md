# PILOT-GALICIA
Repository representing the customizations, specific extensions, and features of Galicia SIMPATICO Pilot

## Pilot Deployment
### Components
The following components are engaged in the Galicia Pilot
- AAC (aac)
- LOG (logs)
- Citizenpedia
- TAE (simpatico-adaptation-engines)
- WAE (simpatico-adaptation-engines)
- CPD 
- CDV
- IFE
- SF
- eSM

Also deployed: replicas for Xunta de Galicia's e-services BS607A, BS611A and BS613B.

### Physical deployment
- Main linux server ``simpatico.hi-iberia.es`` hosting all of the components in the list above. The server runs a virtualized environment using Citrix on top of a rack server physically at HI Iberia's Data Centre. Administrative access to the components done using secure SSH connections accessible only from specific IPs, managed by HI Iberia.

- Access to the replicas (SIMPATICO and control replica without SIMPATICO) is open at https://simpatico.hi-iberia.es:4570/IFE/index_es.html .

## Pilot-specific Customizations
### AAC
- Google login used in the pilot operations.

### IFE
Customizations refer to
- Components engaged: QAE, TAE, CDV and WAE.

### TAE
- Simplification is done only at paragraph level (clicks on paragraphs of the e-service yields simplified output).

### eSM
- e-Service Monitor is available at https://simpatico.hi-iberia.es:4570/esm
- The monitor is username/password protected.
- The data is loaded from the Galicia LOG data currently live on the server.
- The 'SIMPLIFICAR' (simplify) tab is empty and just a placeholder for AST (not deployed in the Galicia pilot).

### WAE
- Version 1.1 deployed.
- Working on all of the e-services using the 'Guía' button on the IFE.
- Displays step-by-step completion guide for the service with inner logic that dictates jumps from one block to the following depending on the answers.
- Displays additional, non legal, text for help for every step.

