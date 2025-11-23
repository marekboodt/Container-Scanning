# Trivy Exception Management

## Overzicht

Deze folder bevat gecentraliseerde exception lists voor Trivy container scanning.

## Structuur

- **global.trivyignore** - Exceptions voor ALLE projecten
- **ubuntu.trivyignore** - Ubuntu base image specifiek
- **alpine.trivyignore** - Alpine base image specifiek
- **node.trivyignore** - Node.js base image specifiek
- **python.trivyignore** - Python base image specifiek

## Exception Levels

### 1. Global Exceptions
Toegepast op alle projecten, gebruik voor:
- Kernel issues zonder fix
- Organisatie-brede beslissingen
- False positives die overal voorkomen

### 2. Base Image Exceptions
Per OS/runtime, gebruik voor:
- OS-specifieke issues
- Base image CVEs zonder patch
- Runtime-specifieke vulnerabilities

### 3. Project Exceptions
In project repo (.trivyignore), gebruik voor:
- Project-specifieke dependencies
- Tijdelijke exceptions
- Context-specifieke issues

## Format
