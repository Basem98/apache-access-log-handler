# ELK Task
Set up a logging and visualization pipeline.

# Requirements:
    ○ Use Logstash to parse an Apache access log file.
    ○ Index the parsed logs into Elasticsearch.
    ○ Create a Kibana dashboard to:
        1. Visualize request count over time.
        2. Filter logs by status code (e.g., 200, 404).
        3. Identify top requested URLs.
    ○ Introduce new service to internal project
        1. Configure rsyslog
        2. Configure logstash
        3. Configure index template, index aliases, ilm policy, inventories, users, roles 
        4. Run required ansible playbooks for ex: roles, users, index aliases, index templates, ilm policies
        5. Create ansible playbooks for managing rsyslog, logstash creation and destruction
        6. Test logs pipeline from rsyslog -> kafka topic -> logstash -> elastic index

