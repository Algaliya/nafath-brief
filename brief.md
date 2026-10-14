Version: NAFATH-V3
Track: <one of: Software | AI | Mobile | Networking | Cybersecurity | Data>

## Overview
A trustworthy government AI assistant depends on several IT fields working together. Software versioning helps developers update the assistant's public API without unexpectedly breaking connected services. Retrieval-Augmented Generation (RAG) allows the AI to use relevant official information when answering citizens. Mobile security protects data exchanged between the app and government servers. Networking provides sufficient addressing capacity and reliable connectivity for growing numbers of devices. Cybersecurity measures help prevent malicious instructions from manipulating the assistant. Data protection practices reduce the privacy risks created by storing chat logs. Together, these controls support a service that is secure, reliable, maintainable, and respectful of citizens' privacy. Clear technical standards and regular verification are essential because incorrect answers or insecure connections could undermine public trust.

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

## Cybersecurity

## Data

## Misconception in My Track

## Open Question
