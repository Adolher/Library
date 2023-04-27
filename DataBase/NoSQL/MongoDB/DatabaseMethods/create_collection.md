<sup>[MongoDB Docs .createCollection()](https://www.mongodb.com/docs/manual/reference/method/db.createCollection/)</sup>

# Create Collection

```mongoDB
db.createCollection( <name>,
   {
     capped: <boolean>,
     timeseries: {
        timeField: <string>,
        metaField: <string>,
        granularity: <string>
     },
     expireAfterSeconds: <number>,
     clusteredIndex: <document>,
     changeStreamPreAndPostImages: <document>,
     size: <number>,
     max: <number>,
     storageEngine: <document>,
     validator: <document>,
     validationLevel: <string>,
     validationAction: <string>,
     indexOptionDefaults: <document>,
     viewOn: <string>,
     pipeline: <pipeline>,
     collation: <document>,
     writeConcern: <document>
   }
)
```

**return**: return-info

- *\<name>*: name of the collection
- (optional) capped *\<boolean>*: default true; [Capped Collections](https://www.mongodb.com/docs/manual/core/capped-collections/)
  - to create a capped collection
- (optional) timeseries: to create a time series collection; [Time Series Collection](https://www.mongodb.com/docs/manual/core/timeseries-collections/)
  - timeseries.timeField *\<string>*: name of the time series field
  - (optional) timeseries.metaField *\<string>*: name of the field which contains metadata
  - (optional) timeseries.granularity *\<string>*: "seconds" (default), "minutes", "hours"
- (optional) expireAfterSeconds *\<number>*: time after which a document expires
- clusteredIndex *\<document>*: [Clustered Collection](https://www.mongodb.com/docs/manual/core/clustered-collections/#std-label-clustered-collections)
- (optional) changeStreamPreAndPostImages *\<document>*: [Change Stream with Document Pre- and Post-Images](https://www.mongodb.com/docs/manual/reference/method/db.collection.watch/#change-streams-with-document-pre--and-post-images)
- (optional) size *\<number>*: the max size of bytes in a capped collection
- (optional) max *\<number>*: the max number of documents in a capped collection
- (optional) storageEngine *\<document>*: [Specify Storage Engine Options](https://www.mongodb.com/docs/manual/reference/method/db.createCollection/#std-label-create-collection-storage-engine-options)
- (optional) validator *\<document>*: specify validation rules; [Schema Validation](https://www.mongodb.com/docs/manual/core/schema-validation/)
- (optional) validationLevel *\<string>*: "off", "strict" (default), "moderate"
- (optional) validationAction *\<string>*: [Choose How to Handle Invalid Documents](https://www.mongodb.com/docs/manual/core/schema-validation/handle-invalid-documents/#choose-how-to-handle-invalid-documents)
- (optional) indexOptionDefaults *\<document>*: to specify a default configuration for indexes
- viewOn *\<string>*: name of the source collection or view
- pipeline *\<array>*: aggregation pipeline stages
- collation *\<document>*: [Collation](https://www.mongodb.com/docs/manual/reference/collation/)
- (optional) writeConcern *\<document>*: [writeConcern](https://www.mongodb.com/docs/manual/reference/write-concern/)

[Examples](https://www.mongodb.com/docs/manual/reference/method/db.createCollection/#example)

---
