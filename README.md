# Tamarin scripts for TEE-based protocols
This is the full repository of Tamarin scripts for the paper "A Symbolic Model for Systematically Analyzing TEE-based protocols" written by Shiwei Xu et al. The scripts in the repository model five following TEE-based protocols:

* Chain of Trust protocol in ARMv8 TF-A
* FIDO2 WebAuthn protocol -- registration phase using the self-attestation scheme
* FIDO2 WebAuthn protocol -- registration phase using the basic-attestation scheme
* FIDO2 WebAuthn protocol -- registration phase using the ECDAA-attestation scheme
* FIDO2 WebAuthn protocol -- authentication phase

Since we consider a detailed threat model, in one folder, there are several scripts capturing different attacker abilities for the same protocol. Due to the complexity of ECDAA attestation scheme, we simplify the protocol to check the unlinkability between authenticators, and the related scripts are in the folder “2.4_FIDO2_WebAuthen_ECDAA_Diff”. All the scripts can be verified by using Tamarin 1.4.1 (https://tamarin-prover.github.io/).
