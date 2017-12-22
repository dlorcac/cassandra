# cassandra
Administracion


# Cassandra - Mantenimiento
# /usr/bin/nodetool
# /var/lib/cassandra/data => Path por default de backups
* Create a Cassandra snapshot for a single node

* To delete all Cassandra snapshots of a node
-- nodetool clearsnapshot


* Create a Cassandra snapshot for a single node - with tag
root@8e8a0024e1ee:~# nodetool snapshot --tag saludos
Requested creating snapshot(s) for [all keyspaces] with snapshot name [saludos] and options {skipFlush=false}
Snapshot directory: saludos

* Delete a Cassandra snapshot for a single node - with tag
root@8e8a0024e1ee:~# nodetool clearsnapshot -t saludos
Requested clearing snapshot(s) for [all keyspaces] with snapshot name [saludos]
