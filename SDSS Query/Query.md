### SQL Query: Joining PhotoObj and SpecObj Tables
This query performs a table `JOIN` between the imaging (`PhotoObj`) and spectra (`SpecObj`) tables, and includes the necessary columns in the `SELECT` clause to upload the results to the Science Archive Server (SAS) for FITS file retrieval.

```sql
SELECT TOP 100000
    p.objid, p.ra, p.dec, p.u, p.g, p.r, p.i, p.z,
    p.run, p.rerun, p.camcol, p.field,
    s.specobjid, s.class, s.z AS redshift,
    s.plate, s.mjd, s.fiberid
FROM PhotoObj AS p
JOIN SpecObj AS s ON s.bestobjid = p.objid
WHERE 
    p.u BETWEEN 0 AND 19.6
    AND p.g BETWEEN 0 AND 20
