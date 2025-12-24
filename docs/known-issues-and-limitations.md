# Limeboard – Known Issues, Limitations & Warnings

**Product:** Limeboard  
**Document type:** Informational (non-contractual)  
**Audience:** Engineering / Prototyping  
**Last updated:** 23/12/2025

---

## 1. Purpose

This document lists known issues, functional limitations, and handling warnings applicable to the current Limeboard reference configuration.

This document is provided for information only.  
It does not define product conformity, acceptance criteria, or warranty obligations.

---

## 2. Known Issues  
*(Current reference software and configuration)*

- The one USB port (top left) out of the four is currently not supported by the kernel.  
  The port is powered, but connected devices are not detected.
- The accelerometer is currently not supported by the kernel.
- The GPU is not initialized in the default reference configuration.
- The board may fail to boot if the FP2 UART is connected to an external device during power-up.   
  The MCU UART is not concerned by this issue.

These issues reflect the current software and configuration state and may change over time.

---

## 3. Functional Limitations

- Cellular (4G) and GNSS functionality require an external antenna, which is not supplied.  
  These interfaces are therefore not functional out of the box.
- The product is intended for use within the European Union only, due to applicable telecommunications frequency and regulatory constraints.

---

## 4. Handling & Manipulation Warnings

- Board configuration (e.g. jumpers) must not be modified while the board is powered, as this may result in permanent hardware damage.
- Improper handling or operation outside the recommended conditions described in the Limeboard datasheet may result in hardware damage.

Reference:  
- Limeboard Datasheet: ../datasheet.md

---

## 5. End-of-Life and Disposal (WEEE)

Limeboard is professional electronic equipment intended for use by engineers and R&D personnel.

It must not be disposed of as unsorted household waste.

At end of life, the product should be:
- returned to appropriate professional electronic waste channels, or
- returned to Citronics for proper reuse, recycling, or treatment.

Citronics may offer a professional take-back option upon request.


## 6. Relationship to Other Documentation

- Hardware conformity is defined exclusively in the Limeboard Hardware Validation Scope document.
- This document complements, but does not replace, the hardware validation scope or the Sales Conditions.

The applicable hardware validation scope is the version published at the time of product delivery.

---

