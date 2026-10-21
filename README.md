# Chatham County STVRs data

Normalized Chatham County parcel and calls-for-service data. This publication includes the 108,191 retained CFS records and parcel records whose mailing normalization status is `normalized` or `repeated_labels_preserved`. Unresolved CFS records and parcel mailing records with blank or ambiguous status are omitted. Repeated mailing addresses and repeated-label parser flags are preserved as requested. The mixed-review Excel workbook is omitted.

CSV parts each have a header. Concatenate their data rows to reconstruct a table. Parcel geometry is preserved in gzip-compressed GeoJSON; decompress it before opening it in a GIS tool. Byte-identical duplicate parcel source copies are represented once.

`publication_manifest.json` lists file checksums, published counts, source quality counts, and omissions. `source_summary.json` and `source_validation.json` describe the original normalization run, including counts for records omitted here; they are not validation results for this filtered publication.

Mailing normalization is syntactic and does not validate deliverability. Property addresses and geometry are preserved. Retained calls include intersection and street-variant candidates: only unique exact matches receive a definitive PIN. Candidate parcels do not establish household involvement, and call records do not establish STVR activity or wrongdoing. Residential classifications include provisional multifamily inferences based on existing project rules.

No license for redistribution is asserted by this publication.
