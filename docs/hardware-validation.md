# Limeboard – Hardware Validation Scope

**Product:** Limeboard  
**Document type:** Hardware validation scope  
**Status:** Informational  
**Audience:** Engineering / Prototyping  
**Last updated:** 23/12/2025 

---

## 1. Purpose

This document defines the hardware validation scope performed on Limeboard prior to shipment.

The purpose of this validation is to confirm basic hardware operability using reference software. 
It does not constitute a guarantee of software behaviour, performance, reliability, or suitability for production use.

---

## 2. Validation Environment

Validation is performed using:
- Citronics reference operating system image
- Citronics reference embedded controller firmware
- Standard Linux-based test environment

The reference software is provided for evaluation and development purposes only.

---

## 3. Validation Scope

The following checks are performed to confirm hardware operability at the time of validation.

### 3.1 Boot and System Bring-Up
- Power-up and reset sequencing
- Boot to operating system userspace

---

### 3.2 Core System Functionality
- CPU detected and operational
- System memory detected and accessible
- Basic OS functionality verified

---

### 3.3 Peripheral Enumeration and Basic Operation

The following peripherals are validated for detection and basic operation:

- Cellular modem (4G) (validated with external antenna; requires customer-provided antenna)
- Wi-Fi
- Bluetooth Low Energy (BLE)
- USB
- Ethernet
- Embedded controller (MCU)
- Debug mode access
- UART
- GPU (validated in a dedicated configuration; not initialized in the default reference setup)
- GNSS / GPS (validated with external antenna; requires customer-provided antenna)
- SD / MMC interface

Validation consists of device detection, enumeration, and basic functional checks.
No performance, throughput, stress, or long-duration testing is performed.

---

## 4. Out of Scope

The following are explicitly out of scope of this validation:

- Application-level behaviour
- Performance benchmarking
- Stability or long-term reliability testing
- Power consumption optimisation
- Environmental or stress testing
- Security validation
- Regulatory or certification compliance
- Customer-specific use cases

---

## 5. Disclaimer

This hardware validation confirms basic operability only.  
It does not constitute:
- an acceptance test for any specific application,
- a warranty of software behaviour,
- a guarantee of production readiness or certification compliance.

Final system validation, integration, and certification remain the sole responsibility of the customer.

---

## 6. Reference

This validation scope is referenced by the Citronics Limeboard Sales Conditions.  
The applicable scope is the version published at the time of product delivery.

