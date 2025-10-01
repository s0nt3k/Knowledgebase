## SMART Attributes

 ***DriveSmartAttributes.json*** is a best-effort, manufacturer-level reference that aggregates commonly observed **SMART/health attributes** for twenty major drive vendors. The file includes a manufacturers array; each manufacturer object lists the vendor name, the device interface types they commonly produce (IDE/SATA/NVMe/SCSI), and an attributes list where each attribute record contains an id (numeric for ATA-style attributes or null for NVMe named fields), a friendly name, a short description, and the types the attribute applies to. It’s intended as a convenience lookup to annotate SMART output (for example, mapping numeric ATA attribute IDs to readable names or matching NVMe health fields), not as an authoritative per-model specification.
 
 **Disclaimer:** SMART attribute implementations and ID assignments vary by vendor, controller, and model manufacturers frequently add vendor-specific attributes, reuse IDs, or expose different NVMe health fields so this JSON should be treated as a helpful starting point rather than a definitive source; always verify critical findings against vendor datasheets, model-specific documentation, or trusted tools like smartmontools/CrystalDiskInfo, and test against the exact drive model before making operational decisions.
 
 ---
