# xendit-kubernetes-config

This is th kubernetes deployment config for the xendit preasessment. This configuration will deploy and provision 4 apps:
1. Comments API, which will provide functionality to post a comment, get a comment, and delete a comment https://github.com/irvanzarkasie/xendit-comment
2. Database adapter, to integrate the API to the mongo db database. This adapter will provide an HTTP API which will enable the comments API to insert, read, and delete data from/to the database. https://github.com/irvanzarkasie/xendit-db
3. Logger API, which will provide functionality to log an information into a text file. It is designed to be the central piece for the logging mechanism. https://github.com/irvanzarkasie/xendit-logger

Once this configuration applied into the kubernetes cluster, the comments API can be invoked via port 30000
