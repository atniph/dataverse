Life Science Metadata block (biomedical.tsv) was updated.  "Other Design Type", "Other Factor Type", "Other Technology Type", "Other Technology Platform" boxes were added. To update the existing Life Science Metadata block run `curl http://localhost:8080/api/admin/datasetfield/load -X POST --data-binary @biomedical.tsv -H "Content-type: text/tab-separated-values"`. To be able to publish one needs to reload solr: copy `schema_dv_mdb_fields.xml` and `schema_dv_mdb_copies.xml` to solr server, for example into /usr/local/solr/solr-7.7.2/server/solr/collection1/conf/ directory and reload the solr, for example, `http://localhost:8983/solr/admin/cores?action=RELOAD&core=collection1`   