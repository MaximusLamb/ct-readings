* First Stage: The $match stage filters the documents by the status field and passes to the next stage those documents that have status equal to "A".

* Second Stage: The $group stage groups the documents by the cust_id field to calculate the sum of the amount for each unique cust_id.

## PIPELINE
* The MongoDB aggregation pipeline consists of stages. Each stage transforms the documents as they pass through the pipeline. Pipeline stages do not need to produce one output document for every input document; e.g., some stages may generate new documents or filter out documents.

* The first stage of the pipeline is matching, and that allows us to filter out documents so that we're only manipulating the documents we care about. The matching expression looks and acts much like the MongoDB find function or a SQL WHERE clause.

* Once we've filtered out the documents we don't want, we can start grouping together the ones that we do into useful subsets. We can also use groups to perform operations across a common field in all documents, such as calculating the sum of a set of transactions and counting documents.

