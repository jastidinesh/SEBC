## Cloudera Manager API Calls

#### Deployment Details :

Command used : `curl -u 'jastidinesh:cloudera' http://ip-172-30-0-87:7180/api/v2/cm/deployment`

Output :
```commandline
{
  "timestamp" : "2017-03-22T23:02:26.520Z",
  "clusters" : [ {
    "name" : "jastidinesh",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "550502400"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "550502400"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "3432356249"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "577"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "172.30.0.87"
        }, {
          "name" : "hive_metastore_database_name",
          "value" : "hive"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive_password"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-0c353764b393666143d827c0229a28ac",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0cd04073b63356e7c"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-1d0a2cd59670c30888770429877d4b85",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0fa86eb3b81e48b25"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-33505bab7e5ceb85bc5b303eeb46db8a",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0648c332cfb8d576a"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-6f585328281f0cdf5b0dc924c1942a45",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0b4a75cc90e30aaff"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-d14d08f4f78fc2137a9c8e202e00ee3b",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0d32395f455dbbe67"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-0c353764b393666143d827c0229a28ac",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "i-0cd04073b63356e7c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4srcwnp8v0vsglxuewpde99hk"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-0c353764b393666143d827c0229a28ac",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "i-0cd04073b63356e7c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8bum1iqsu6iqzr7mpp80jyys"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SERVER",
          "items" : [ {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "550502400"
          } ]
        } ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-0c353764b393666143d827c0229a28ac",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-0cd04073b63356e7c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2044tvhr68jsmtccldsse9osm"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-33505bab7e5ceb85bc5b303eeb46db8a",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-0648c332cfb8d576a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5cbt4ooaupia2ye301gbadehx"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-d14d08f4f78fc2137a9c8e202e00ee3b",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-0d32395f455dbbe67"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7798zhbg3rcjxxk06wjuwazgt"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "172.30.0.87"
        }, {
          "name" : "database_password",
          "value" : "hue_password"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-HTTPFS-0c353764b393666143d827c0229a28ac"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-0c353764b393666143d827c0229a28ac",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "i-0cd04073b63356e7c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "74vp977ko8xfw0i55kcjr5vd1"
          }, {
            "name" : "secret_key",
            "value" : "F4JP0ARfrnuk6hVnENpHP7Guo2fxmO"
          } ]
        }
      } ],
      "displayName" : "Hue"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "172.30.0.87"
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie_password"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "550502400"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-0c353764b393666143d827c0229a28ac",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "i-0cd04073b63356e7c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "854wp6grzknpvi3xl76fsi49f"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "8"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "550502400"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "4939"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "resource_manager_java_heapsize",
            "value" : "550502400"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "4939"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "3"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "90"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "6e1tomYLGyfu51xTamrnwAXmaZMKV8"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-0c353764b393666143d827c0229a28ac",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "i-0cd04073b63356e7c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "b7m9rbb5cdkggwfdtkfff7k7g"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-1d0a2cd59670c30888770429877d4b85",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0fa86eb3b81e48b25"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1ozu08rp8ao5bjuzhyfovdnol"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-33505bab7e5ceb85bc5b303eeb46db8a",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0648c332cfb8d576a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2l0meefc1vpytk2orgy5kkqgp"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-6f585328281f0cdf5b0dc924c1942a45",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0b4a75cc90e30aaff"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ajs27jn44f8rcu82aqhb58dzd"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-d14d08f4f78fc2137a9c8e202e00ee3b",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0d32395f455dbbe67"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5div0toc658qh4dd4mf4wv7k3"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-0c353764b393666143d827c0229a28ac",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "i-0cd04073b63356e7c"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "85"
          }, {
            "name" : "role_jceks_password",
            "value" : "e0191cqvednemlncjai7yuji8"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "BALANCER",
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "550502400"
          } ]
        }, {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "3219866009"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "200"
          }, {
            "name" : "rm_io_weight",
            "value" : "100"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/dfs/jn"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "550502400"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "550502400"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "TMmhfcdr3iyLL81bqHg3YmZviof5hP"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "CjnkgHkP15rPRcjMpefek4q2GzPBki"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "bNJkR2XWeWShGJf48quy3TymdjOr1b"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "10"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-0c353764b393666143d827c0229a28ac",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "i-0cd04073b63356e7c"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-1d0a2cd59670c30888770429877d4b85",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0fa86eb3b81e48b25"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "e9dwlomrqzu57jsuptnwhdvba"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-33505bab7e5ceb85bc5b303eeb46db8a",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0648c332cfb8d576a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6zd2x7yesq7rdqosv3be50scj"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-6f585328281f0cdf5b0dc924c1942a45",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0b4a75cc90e30aaff"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1rizoewatj5cklqm04dfphg8z"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-d14d08f4f78fc2137a9c8e202e00ee3b",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0d32395f455dbbe67"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "78tz9bmzbgw4boqbcl947x7k6"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-0c353764b393666143d827c0229a28ac",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "i-0cd04073b63356e7c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "aplntxwz14kvf5pfdexii0apo"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-d14d08f4f78fc2137a9c8e202e00ee3b",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "i-0d32395f455dbbe67"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7uu11h2v31mc0e11wpxjpspah"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-0c353764b393666143d827c0229a28ac",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "i-0cd04073b63356e7c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6z18eddks6zs7mfc1h1ih3sv3"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-0c353764b393666143d827c0229a28ac",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-0cd04073b63356e7c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "b8elkw52oxwunqo2ij5h0vtyy"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-33505bab7e5ceb85bc5b303eeb46db8a",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-0648c332cfb8d576a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1rn2i4p98lz31084g95owmhgr"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-d14d08f4f78fc2137a9c8e202e00ee3b",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-0d32395f455dbbe67"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9wsoe55cn72ovlhf9c0dx6w0p"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-0c353764b393666143d827c0229a28ac",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "i-0cd04073b63356e7c"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "hdfsHA"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "hdfsHA"
          }, {
            "name" : "namenode_id",
            "value" : "87"
          }, {
            "name" : "role_jceks_password",
            "value" : "de1i4wulj3zgg1qxv9vx03pz8"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-d14d08f4f78fc2137a9c8e202e00ee3b",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "i-0d32395f455dbbe67"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "hdfsHA"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "hdfsHA"
          }, {
            "name" : "namenode_id",
            "value" : "93"
          }, {
            "name" : "role_jceks_password",
            "value" : "7wrn71zyglppl88yjj4j8wdk3"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "i-0fa86eb3b81e48b25",
    "ipAddress" : "172.30.0.103",
    "hostname" : "ip-172-30-0-103.ec2.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0b4a75cc90e30aaff",
    "ipAddress" : "172.30.0.153",
    "hostname" : "ip-172-30-0-153.ec2.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0648c332cfb8d576a",
    "ipAddress" : "172.30.0.6",
    "hostname" : "ip-172-30-0-6.ec2.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0d32395f455dbbe67",
    "ipAddress" : "172.30.0.65",
    "hostname" : "ip-172-30-0-65.ec2.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0cd04073b63356e7c",
    "ipAddress" : "172.30.0.87",
    "hostname" : "ip-172-30-0-87.ec2.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-ACTIVITYMONITOR-0c353764b393666143d827c0229a28ac",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "5958dfcbe697cc33d1aec0b54563b7da7642e757cfa47df1e32c97297bb58654",
    "pwSalt" : 9143647416458183002,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-0c353764b393666143d827c0229a28ac",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "12cdc84fe41ec34d656c5001b6f24ea46628f94de114ef1ee551ab886b1f7738",
    "pwSalt" : 7167415010887442232,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-0c353764b393666143d827c0229a28ac",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "8e412df7abf2d1dd455db39fdd69ac5cec37bfb5130f2c1743a4454dedc38252",
    "pwSalt" : -544786827759996548,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-0c353764b393666143d827c0229a28ac",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "a4b0775f85eadadb22fa36c00111c1a086d6552168f3f0acad44b4894be37dfa",
    "pwSalt" : 4138061678642648564,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-0c353764b393666143d827c0229a28ac",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "88edd5cd80e9eca781665db5e454c64aa2e5c05d21273be68d0ef70273b62449",
    "pwSalt" : 9132978530219887515,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "2f2e206610ee3d95fe9e55c9195f6ddd99ac876c151c6b775965586d4ac7bba5",
    "pwSalt" : -5865443868990210109,
    "pwLogin" : true
  }, {
    "name" : "jastidinesh",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "62d712c0fdf73e477ee2b659d5f79685f0ce23dd7471765fcd71a72167dd8f63",
    "pwSalt" : -7905277541690999932,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "f929b2f6b65e2d94ce3d0713f36d2a808c01b83e47e6126d27471797418b63aa",
    "pwSalt" : 785307834953000823,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.9.1",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170112-1158",
    "gitHash" : "a66d8bbdbe8bc3ee54235e55423f2f76c7d9f3b1",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "ACTIVITYMONITOR",
        "items" : [ {
          "name" : "firehose_database_host",
          "value" : "172.30.0.87"
        }, {
          "name" : "firehose_database_name",
          "value" : "amon"
        }, {
          "name" : "firehose_database_password",
          "value" : "amon_password"
        }, {
          "name" : "firehose_database_user",
          "value" : "amon"
        }, {
          "name" : "firehose_heapsize",
          "value" : "550502400"
        } ]
      }, {
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "550502400"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "172.30.0.87"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman_password"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "550502400"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ACTIVITYMONITOR-0c353764b393666143d827c0229a28ac",
      "type" : "ACTIVITYMONITOR",
      "hostRef" : {
        "hostId" : "i-0cd04073b63356e7c"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "94a4598mgi64dk9jqot0dltf5"
        } ]
      }
    }, {
      "name" : "mgmt-ALERTPUBLISHER-0c353764b393666143d827c0229a28ac",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "i-0cd04073b63356e7c"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9tse7gscqwqh50m6uwevtp2b7"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-0c353764b393666143d827c0229a28ac",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "i-0cd04073b63356e7c"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "79gb2zvnwoyixc0htl8ivuf92"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-0c353764b393666143d827c0229a28ac",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "i-0cd04073b63356e7c"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "dp5wi0m4v5ar283y2icwvphbm"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-0c353764b393666143d827c0229a28ac",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "i-0cd04073b63356e7c"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "5dulw4ht783dvvk3r2sg9n3bq"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-0c353764b393666143d827c0229a28ac",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "i-0cd04073b63356e7c"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "5vts2zzr9ylv8590xcua3udsw"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/27/2012 12:40"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,http://ip-172-30-0-87.ec2.internal/cdh5.9.1/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    } ]
  }
}
```

