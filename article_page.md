# Articles
Articles are created for displaying the content of reports. When a user open a report, at least one **article** is created. An article's content can be a paragraph and one graph or one table.

## Tables and graphs REST access

### Table 1 REST
**Request url:**
	GET /api/DataFeeds/get_client_performance/:employer_brand_id/:channel/:year/:edition_short_name   return Table 1
	
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name              | Required | Format | Description
----------------- | -------- | ------ | ---
employer_brand_id | required | int    | 
channel           | required | string |
year              | required | int    |
edition_short_name| required | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

### Table 2 REST
**Request url:**
	GET /api/rankdata/api_rankings/:edition_shortname/:topic/:year   return Table 2

**Header:**

	Content-Type: application/json
  
**JSON:** none

Name              | Required | Format | Description
----------------- | -------- | ------ | ---
employer_brand_id | required | int    | 
topic             | required | string |
year              | required | int    |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

### Table 3 REST
**Request url:**
	GET /api/DataFeeds/get_ranking_section/:surveyfeatures_channel/:section_id/:edition_short_name/:employer_brand_id/:benchmarks

**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                   | Required | Format | Description
---------------------- | -------- | ------ | -----------
surveyfeatures_channel | required | string | 
section_id             | required | int    |
edition_short_name     | required | string |
employer_brand_id      | required | int    |
benchmarks             | required | string | a string with benchmarks which is separated by comma

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 


### Table 4 REST
**Request url:**
	GET /api/DataFeeds/get_max_score_section/:surveyfeatures_channel/:section_id/:edition_short_name/:employer_brand_id   return Table 4

**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                   | Required | Format | Description
---------------------- | -------- | ------ | -----------
surveyfeatures_channel | required | string | 
section_id             | required | int    |
edition_short_name     | required | string |
employer_brand_id      | required | int    |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 


### Table 5 REST
**Request url:**
	GET /api/DataFeeds/get_feature_importance_in_section/:employer_brand_id/:surveyfeatures_channel/:year/:edition_short_name/:section_id   return Table 5
	
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                   | Required | Format | Description
---------------------- | -------- | ------ | -----------
employer_brand_id      | required | int    | 
surveyfeatures_channel | required | string |
year                   | required | int    |
edition_short_name     | required | string |
section_id             | required | int    |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 8 REST
**Request url:**	
	GET /api/DataFeeds/get_features_benchmarks/:employer_brand_id/:surveyfeatures_channel/:year/:edition_short_name/:employer_brand_benchmarks   return Table 

**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                      | Required | Format | Description
------------------------- | -------- | ------ | -----------
employer_brand_id         | required | int    | 
surveyfeatures_channel    | required | string |
year                      | required | int    |
edition_short_name        | required | string |
employer_brand_benchmarks | required | string | a string with benchmarks which is separated by comma

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 9 REST
**Request url:**
	GET /api/DataFeeds/get_company_url/:year/:channel_id/:edition_short_name/:employer_brand_id_benchmark   return Table 9
	
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
year                        | required | int    |
channel_id                  | required | int    | 
edition_short_name          | required | string |
employer_brand_id_benchmark | required | string | a string with benchmarks which is separated by comma

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 


### Table 10 REST
**Request url:**
	GET /api/DataFeeds/get_matrix_missing_features/:employer_brand_id/:topic/:year/:edition_short_name   return Table 10
		
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
employer_brand_id           | required | int    | 
topic                       | required | string |
year                        | required | int    |
edition_short_name          | required | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 12 REST
**Request url:**
	GET /api/DataFeeds/get_ranking_some_channel/:employer_brand_id/:surveyfeatures_channel/:edition_short_name/:year   return Table 11
		
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
employer_brand_id           | required | int    | 
surveyfeatures_channel      | required | string |
edition_short_name          | required | string |
year                        | required | int    |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 13 REST
**Request url:**
	GET /api/DataFeeds/get_ranking_features_some_channel/:employer_brand_id/:surveyfeatures_channel/:year/:edition_short_name   return Table 12
	
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
employer_brand_id           | required | int    | 
surveyfeatures_channel      | required | string |
year                        | required | int    |
edition_short_name          | required | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 14 REST
**Request url:**
	GET /api/DataFeeds/get_features_benchmarks_some/:employer_brand_id/:channel/:year/:edition_short_name/:employer_brand_benchmarks   return Table 14
	
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
employer_brand_id           | required | int    | 
channel                     | required | string |
year                        | required | int    |
edition_short_name          | required | string |
employer_brand_benchmarks   | required | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 15 REST
**Request url:**
	GET /api/rankdata/get_ranking_benchmarks/:edition_shortname/:topic/:year/:benchmark_ids_string   return Table 15

**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
edition_short_name          | required | string |
topic                       | required | int    | 
year                        | required | int    |
benchmark_ids_string        | required | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 17 REST
**Request url:**
	GET /api/DataFeeds/get_industry_ranking/:year/:topic/:edition_short_name/:employer_brand_id   return Table 17
	
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
year                        | required | int    |
topic                       | required | string |
edition_short_name          | required | string |
employer_brand_id           | required | int    | 

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 20 REST
**Request url:**
	GET /api/DataFeeds/get_email_testing_facebook/:employer_brand_id/:year/:edition_short_name/:employer_brand_benchmarks   return Table 20
	
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
employer_brand_id           | required | int    | 
year                        | required | int    |
edition_short_name          | required | string |
employer_brand_benchmarks   | required | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 22 REST
**Request url:**
	GET /api/DataFeeds/get_table_missing_features_some_channel/:employer_brand_id/:surveyfeatures_channel/:year/:edition_short_name   return Table 22
	
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
employer_brand_id           | required | int    | 
surveyfeatures_channel      | required | string |
year                        | required | int    |
edition_short_name          | required | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 23 REST
**Request url:**
	GET /api/DataFeeds/get_client_performance_some_channel/:employer_brand_id/:surveyfeatures_channel/:year/:edition_short_name   return Table 23
	
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
employer_brand_id           | required | int    | 
surveyfeatures_channel      | required | string |
year                        | required | int    |
edition_short_name          | required | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	  
### Table 26 REST
**Request url:**
	GET /api/Data_feeds/get_missing_feat_gl_sum/:employer_brand_id/:channel/:year/:edition_short_name/:employer_brand_benchmarks   return Table 26
	
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required   | Format | Description
--------------------------- | ---------- | ------ | -----------
employer_brand_id           | required   | int    | 
channel                     | required   | string |
year                        | required   | int    |
edition_short_name          | required   | string |
employer_brand_benchmarks   | no require | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 45 REST
**Request url:**
	GET /api/DataFeeds/get_table_20_missing_features/:employer_brand_id/:surveyfeatures_channel/:year/:edition_short_name   return Table 45
	
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
employer_brand_id           | required | int    | 
surveyfeatures_channel      | required | string |
year                        | required | int    |
edition_short_name          | required | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	 
### Table 36 REST
**Request url:**
	GET /api/DataFeeds/get_channel_company_ranking/:edition_short_name/:employer_brand_id   return Table 36

**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
edition_short_name          | required | string |
employer_brand_id           | required | int    | 

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	  
### Table 37 REST
**Request url:**
	GET /api/DataFeeds/get_graph_company_ranking_bench/:topic/:edition_short_name/:employer_brand_id/:benchmarks   return Table 37
	
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
topic                       | required | string | 
edition_short_name          | required | string |
employer_brand_id           | required | int    |
benchmarks                  | required | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 38 REST
**Request url:**
	GET /api/DataFeeds/get_graph_company_ranking_edition/:topic/:employer_brand_id   return Table 38
	
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
topic                       | required | string | 
employer_brand_id           | required | int    |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 


### Table 39 REST
**Request url:**
	GET /api/DataFeeds/get_graph_cat_company_ranking_ed/:year/:employer_brand_id/:employer_brand_id_benchmark/:edition_short_name/:channel   return Table 39
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
year                        | required | int    |
employer_brand_id           | required | int    | 
employer_brand_id_benchmark | required | string |
edition_short_name          | required | string |
channel                     | required | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 40 REST
**Request url:**
	GET /api/DataFeeds/get_graph_cat_company_ranking_ed_some/:year/:employer_brand_id   return Table 40

**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
year                        | required | int    | 
employer_brand_id           | required | int |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 41 REST
**Request url:**
	GET /api/DataFeeds/get_some_overview_topic/:year/:edition_short_name   return Table 41

**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
year                        | required | int    | 
edition_short_name          | required | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 42 REST
**Request url:**
| GET      | /api/DataFeeds/get_graph_cat_company_rank_bench/:year/:employer_brand_id/:employer_brand_id_benchmark/:edition_short_name/:channel   return Table 42
**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
employer_brand_id           | required | int    | 
surveyfeatures_channel      | required | string |
year                        | required | int    |
edition_short_name          | required | string |
channel                     | required | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

	
### Table 43 REST
**Request url:**
	GET /api/DataFeeds/get_graph_cat_company_rank_bench_some/:year/:employer_brand_id/:employer_brand_id_benchmark/:edition_short_name   return Table 43

**Header:**

	Content-Type: application/json
  
**JSON:** none

Name                        | Required | Format | Description
--------------------------- | -------- | ------ | -----------
year                        | required | int    |
employer_brand_id           | required | int    | 
employer_brand_id_benchmark | required | string |
edition_short_name          | required | string |

**Request:**

```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 

### Trend Graphs REST
**Request url:**
	POST /api/api_trends/trend_response.json   return one of 3 types of graphs (BCP type, BCA type and CC type)
	
**Header:**

	Content-Type: application/json
  
**JSON:** none

**Request:**
{
	"question": {
		"filter_edition": "FR",
		"filter_channel": "some",
		"question": "3027",
		"filter_years": ["2017"]
	}
}
```

**Response Messages:**

HTTP Status Code | Reason | Response Model
-------- | --- | ---
400| Validation error: items do not fit the schema | 
404| No item corresponds to the request | 
