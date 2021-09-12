---
layout: col-sidebar
title: OWASP Application Security Misconfiguration
site_side: true
tags: application-security-misconfiguration
level: 4
type: documentation
auto-migrated: 0
pitch: The primary goal of the OWASP Application Security Misconfiguration document is to provide assistance and education for organizations looking to harden Applications securely. The documents are provides information about what are the most prominent security risks for applications security misconfiguration, the challenges involved, and how to overcome them.
---
## Overview
The Application security misconfiguration arises when security settings are defined, implemented and mantained as default. To protect application, database, server, web app and platform, we should be handled properly. <br>
<br>
The misconfiguration could affect any layer of application stack, network layer and cloud applications. Some of the unsafe features like debug and QA features enabled by default and these features may provide a means for attacker bypass authentication methods and gain access of sensitives information.
## Interim List of Risks - Currently Under Review!

The OWASP Commons Misconfiguration vulnerabilities are currently under development (Sept 2021). As part of our effort to collect feedback, we are presenting an interim list below. Please feel free to contact the project leaders if you have any feedback. 

#### ASM-1: Application's Default Account And Password
Examples:
 * Publicly open s3 bucket
 * Container runs as root
 * Container shares resources with the host (network interface, etc.)
 * Unauthenticated orchestrator console access 
 * Unauthrized or overly-permissive orchestrator access
 * Insecure Infrastructure-as-Code (IaC) configuration
 * Lack of orchestrator node trust rules (e.g. unauthorized hosts joining the cluster)
 * ...

#### ASM-2: Application's Deprecated Protocols
Examples:
 * SQL injection
 * XXE
 * NoSQL injection
 * OS command injection
 * Serverless event data injection
 * ...

#### ASM-3: Application's Weak Ciphers
Examples:
 * Unauthenticated API access on a microservice
 * Over-permissive cloud IAM role
 * ... 

#### ASM-4: Deprecated Encryption methods and algorithme
Examples:
 * Insufficient authentication on CI/CD pipeline systems
 * Use of untrusted images 
 * Use of stale images
 * Insecure communication channels to registries
 * Overly-permissive registry access 
 * Using a single environment to run CI/CD tasks for projects requiring different levels of security
 * ...

#### ASM-5: Insecure secrets storage
Examples:
 * Orchestrator secrets stored unencrypted
 * API keys or passwords stored unencrypted inside containers
 * Hardcoded application secrets
 * Poorly encrypted secrets (e.g. use of obsolete encryption methods, use of encoding instead of encryption, etc.) 
 * Mounting of storage containing sensitive information
 * ...

#### ASM-6: Enabled Default Debug Logs, That Revealing Sensitive Information
Examples:
 * Over-permissive pod to pod communication allowed
 * Internal microservices exposed to the public Internet
 * No network segmentation defined
 * End-to-end communications not encrypted
 * Network traffic to unknown or potentially malicious domains not monitored and blocked
 * ...
#### ASM-7: Services and Ports are enabled to default installation
Examples:
 * Vulnerable 3rd party open source packages
 * Vulnerable versions of application components
 * Use of known vulnerable container images
 * ...

#### ASM-8: Files and directories are unprotected	
Examples:
 * Undocumented microservices & APIs
 * Obsolete & unmanaged cloud resources
 * ...

#### ASM-9: Open Database Instances
Examples:
 * Resource-unbound containers
 * Over-permissive request quota set on APIs
 * ...

#### ASM-10: Outdated Installed Software and flaws are unpatched	
Examples:
 * No container or host process activity monitoring
 * No network communications monitoring among microservices
 * No resource consumption monitoring to ensure availability of critical resources
 * Lack of monitoring on orchestration configuration propagation and stale configs
 * ...

## Getting Involved
we welcome any type of suggestion and comments. Possible ways to contribute:
 * We are actively looking for organizations and individuals that will provide applications security settings and options
 * Individuals and organizations that will contribute to the project will be listed on the acknowledgments page.

## Project Sponsors
The OWASPApplication Security Misconfigurationproject is supported by [Niah Security](https://niahsecurity.io)
<br>
[![N|Solid](http://cyberthreatinfo.expert/static/logo.png)](https://nodesource.com/products/nsolid)
