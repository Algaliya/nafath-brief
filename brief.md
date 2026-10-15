Version: NAFATH-V3
Track: Cybersecurity

## Overview
A trustworthy government AI assistant depends on several IT fields working together. Software versioning helps developers update the assistant's public API without unexpectedly breaking connected services. Retrieval-Augmented Generation (RAG) allows the AI to use relevant official information when answering citizens. Mobile security protects data exchanged between the app and government servers. Networking provides sufficient addressing capacity and reliable connectivity for growing numbers of devices. Cybersecurity measures help prevent malicious instructions from manipulating the assistant. Data protection practices reduce the privacy risks created by storing chat logs. Together, these controls support a service that is secure, reliable, maintainable, and respectful of citizens' privacy. Clear technical standards and regular verification are essential because incorrect answers or insecure connections could undermine public trust. For the Cybersecurity track, prompt injection requires layered safeguards and ongoing testing to protect public trust

## Software
Semantic Versioning uses MAJOR.MINOR.PATCH numbers to communicate changes to the assistant's public API. A MAJOR version must increase when a change breaks backward compatibility. A MINOR version increases when new functionality is added without breaking existing clients. A PATCH version increases for backward-compatible bug fixes. Following these rules helps mobile apps and other services integrate with the assistant safely.
Resource: <Semantic Versioning 2.0.0> - <https://semver.org/spec/v2.0.0.html>
## AI
Retrieval-Augmented Generation (RAG) retrieves relevant information from an external knowledge source and provides it to the language model when generating an answer. For a government assistant, this source could contain current service rules and official guidance. RAG can improve factual accuracy and make answers easier to verify, but it cannot guarantee correctness if the retrieved information is incomplete or the model misuses it.
Resource: <Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks> - <https://proceedings.neurips.cc/paper_files/paper/2020/hash/6b493230-Abstract.html>
## Mobile
Apple's App Transport Security (ATS) requires secure HTTPS connections with appropriate TLS protection when apps use the standard URL Loading System. If an app attempts a plain HTTP request, ATS normally blocks it and reports the insecure connection. Developers should secure the server rather than disable ATS protections. Limited exceptions are possible, but they reduce security and should be used cautiously.
Resource: <Preventing Insecure Network Connections> - <https://developer.apple.com/documentation/security/preventing-insecure-network-connections>
## Networking
IPv4 uses 32-bit addresses, while IPv6 uses 128-bit addresses, providing a vastly larger address space. This matters as governments connect more phones, sensors, servers and other devices. IPv6 supports continued growth and reduces pressure on the limited IPv4 address pool. However, deployment planning must still consider compatibility with existing IPv4 systems, security controls and network configuration.
Resource: <RFC 8200 - Internet Protocol, Version 6 (IPv6) Specification> - <https://www.rfc-editor.org/rfc/rfc8200>
## Cybersecurity
A common misconception is that prompt injection can be completely prevented by telling the AI to ignore malicious instructions. In reality, attackers may hide instructions in external content, such as retrieved webpages or documents, which the AI processes as part of its task. A safer approach combines treating external content as untrusted, limiting the AI's permissions, and testing the system against attacks. No single instruction or defence guarantees complete protection.
Supporting quotation: "there is no fool-proof prevention within the LLM"
Resource: <OWASP Top 10 for LLM Applications - LLM01: Prompt Injection> - <https://genai.owasp.org/llmrisk/llm01-prompt-injection/>
## Data
Anonymisation irreversibly removes the ability to identify a person, considering information reasonably likely to be used for re-identification. Pseudonymization replaces identifying details with substitutes, but a person may still be identified using additional information. Properly anonymised data may fall outside data protection law, while pseudonymized data remains personal data under the GDPR. The classification depends on whether identification is realistically possible.
Resource: <General Data Protection Regulation (GDPR) - Article 4(5) and Recital 26> - <https://eur-lex.europa.eu/eli/reg/2016/679/oj>
## Misconception in My Track
A common misconception is that prompt injection can be completely prevented by telling the AI to ignore malicious instructions. In reality, attackers may hide instructions in external content, such as retrieved webpages or documents, which the AI processes as part of its task. A safer approach combines treating external content as untrusted, limiting the AI's permissions, and testing the system against attacks. No single instruction or defence guarantees complete protection.OWASP's guidance states that “there is no fool-proof prevention within the LLM” and recommends measures to mitigate prompt injection
Resource evidence: <OWASP Top 10 for LLM Applications, LLM01: Prompt Injection> - <https://genai.owasp.org/llmrisk/llm01-prompt-injection/>
## Open Question
How can a government AI assistant distinguish malicious instructions hidden in official-looking documents from legitimate service guidance, while still providing accurate answers and protecting citizens' data?
