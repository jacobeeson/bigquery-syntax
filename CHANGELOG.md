# Changelog

## [1.1.0] - 2026-01-10

### Added
- **AI Functions (16 new functions)** - New `AI.*` function category for AI/ML operations
  - AI.CLASSIFY, AI.DETECT_ANOMALIES, AI.EMBED, AI.EVALUATE
  - AI.FORECAST, AI.GENERATE, AI.GENERATE_BOOL, AI.GENERATE_DOUBLE
  - AI.GENERATE_EMBEDDING, AI.GENERATE_INT, AI.GENERATE_TABLE, AI.GENERATE_TEXT
  - AI.IF, AI.SCORE, AI.SEARCH, AI.SIMILARITY

- **ML Functions (62 new functions)** - Expanded machine learning capabilities
  - Data preprocessing: ML.BUCKETIZE, ML.IMPUTER, ML.MIN_MAX_SCALER, ML.STANDARD_SCALER, ML.ROBUST_SCALER, ML.MAX_ABS_SCALER, ML.NORMALIZER, ML.POLYNOMIAL_EXPAND, ML.QUANTILE_BUCKETIZE
  - Feature engineering: ML.FEATURE_CROSS, ML.FEATURE_INFO, ML.HASH_BUCKETIZE, ML.LABEL_ENCODER, ML.MULTI_HOT_ENCODER, ML.ONE_HOT_ENCODER
  - Text processing: ML.NGRAMS, ML.BAG_OF_WORDS, ML.TF_IDF
  - Image processing: ML.CONVERT_COLOR_SPACE, ML.CONVERT_IMAGE_TYPE, ML.DECODE_IMAGE, ML.RESIZE_IMAGE, ML.ANNOTATE_IMAGE
  - Model evaluation: ML.CONFUSION_MATRIX, ML.ROC_CURVE, ML.ARIMA_EVALUATE, ML.RECONSTRUCTION_LOSS, ML.EVALUATE
  - Model explanation: ML.EXPLAIN_PREDICT, ML.EXPLAIN_FORECAST, ML.GLOBAL_EXPLAIN, ML.FEATURE_IMPORTANCE, ML.ADVANCED_WEIGHTS, ML.WEIGHTS
  - Model components: ML.CENTROIDS, ML.PRINCIPAL_COMPONENTS, ML.PRINCIPAL_COMPONENT_INFO, ML.ARIMA_COEFFICIENTS
  - Data operations: ML.FEATURES_AT_TIME, ML.ENTITY_FEATURES_AT_TIME, ML.TRANSFORM
  - Validation: ML.DESCRIBE_DATA, ML.VALIDATE_DATA_DRIFT, ML.VALIDATE_DATA_SKEW, ML.TFDV_DESCRIBE, ML.TFDV_VALIDATE
  - Prediction: ML.FORECAST, ML.RECOMMEND, ML.DETECT_ANOMALIES
  - Text/Document: ML.UNDERSTAND_TEXT, ML.TRANSLATE, ML.PROCESS_DOCUMENT, ML.TRANSCRIBE, ML.GENERATE_TEXT, ML.GENERATE_EMBEDDING
  - Training: ML.TRAINING_INFO, ML.TRIAL_INFO, ML.HOLIDAY_INFO, ML.GET_INSIGHTS
  - Distance: ML.DISTANCE, ML.LP_NORM

- **Object Storage Functions (3 new functions)** - New `OBJ.*` function category
  - OBJ.FETCH_METADATA, OBJ.GET_ACCESS_URL, OBJ.MAKE_REF

- **BI Functions (2 new functions)** - BI capacity monitoring
  - BI_CAPACITIES, BI_CAPACITY_CHANGES

- **Vector Search (1 new function)** - Vector index statistics
  - VECTOR_INDEX.STATISTICS

### Summary
- Total functions increased from 407 to 489 (+82 functions)
- Grammar now supports latest BigQuery features as of January 2026
- Source: Google Cloud BigQuery Standard SQL documentation

## [1.0.0] - 2026-01-10

### Added
- Initial release
- ~400 BigQuery Standard SQL functions across 18 categories
- Complete data type support (INT64, FLOAT64, STRING, BYTES, DATE, TIME, DATETIME, TIMESTAMP, INTERVAL, GEOGRAPHY, JSON, RANGE, ARRAY, STRUCT)
- All string literal formats (single, double, raw, bytes, multi-line)
- Parameter (@param) and system variable (@@var) highlighting
- Backtick-quoted identifier support
- Comment styles: --, #, /* */
- File associations: .bq, .bqsql
