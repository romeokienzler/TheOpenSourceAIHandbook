# Motivation
In the storage layer we want to build a data lake which simplifies data ingestion, data lifecycle management, data access rights and data access. We think SQL is the best interface when it comes to querying data as the technology is widely adopted and supported by a rich tool set and skilled practitioners

The also think that the SQL layer which sits on top of the storage layer needs to provide a JDBC and ODBC interface to maximize flexibility. In addition, it has to implement the ANSI SQL standard.

We strongly belive that S3 is a de-facto standard when it comes to cheap but reliable storage access. All major cloud proviers offer S3 compatible object storage at very low prices. In addition, open source technologies like [Ceph](https://ceph.io/) bring S3 to the local data center making it a suitable component for the hybrid cloud.
