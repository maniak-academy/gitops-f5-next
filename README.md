# gitops-f5-next

curl -k -X POST -H "Authorization: Bearer 5pQhve6gXZTUs+cj2qEWT2T3hU3LcuwgRZeYajQTbWAr2hObBL29Tsj/OKfgP4oxVltC9C0QlTwZpVmWd9xbDI7uZfaEXt3T8gpscdCJl1BQDmYUrjIC5ioHDWKN/w1xu9mp9Yq1VWrHSSiaqORDKVh60IjkgrrQ6z86RBy/GmMX2PaNhZXQHBjxgOSDmEhX31a7FV+8ev6bfEt/2sfSiYfDqTLQ4MoX54AFGn8sRrHr7wC8KNmUww5nWhnVXnfQ3tzIG0WRMhK6sH5tUDYP4kBMXVHD9sKaTVMFEMaoqpbcPfj9cD2nxFjpaN31DdU9PEKiKgfM55CsRzahM8x1VXMy1J5Xp9Yv1qMl1od9wZ6M4WCu4FSDpGsjZFRUXpv989ODt/5FfdFBqFJ6myx4Gw+Y6VI7M6ip17MhBAZyAYNRYN00EafPLpCWyi6XdzaliGy+DUatkQ3Y19fOo115YeLsrIlts8byAhEvkWKg1Y50aZtbJ8GBwIqpTPxbhHbS8kOBDBpI8xmgj6ZcqsK2goUw8m3zGlzRWcHXWJ/n7A==" "https://172.16.10.67/api/v1/spaces/default/appsvcs/documents" -H "Content-Type: application/json" -d '{ "class": "ADC", "schemaVersion": "3.12.0", "DemoTenant": { "class": "Tenant", "TestApp": { "class": "Application", "template": "http", "serviceMain": { "pool": "Pool", "snat": "auto", "virtualPort": 80, "virtualAddresses": [ "5.6.7.8" ], "class": "Service_HTTP" }, "Pool": { "members": [ { "servicePort": 80, "serverAddresses": [ "5.6.7.8" ] } ], "loadBalancingMode": "round-robin", "class": "Pool" } } } }'
