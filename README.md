A "code-intent pair" dataset containing 26 secure code auditing intent categories, comprising 26,000 functions for training and 4,830 for testing

## intent intent categories

- A_user_identity
  - "user_registration"
  - "user_login"
  - "user_logout"
  - "permission_check"
  - "token_or_session_handling"
  - "verification_sms_email_captcha"

- B_core_business
  - "order_or_payment_operation"
  - "file_upload"
  - "file_download"
  - "search_or_pagination"
  - "config_change"
  - "workflow_or_status_update"
  - "crud_operation"
  - "sensitive_user_action"
  - "business_report_query"

- C_data_resource_access
  - "sql_execution"
  - "orm_operation"
  - "cache_access"
  - "filesystem_access"
  - "command_execution"
  - "internal_service_rpc_call"
  - "transaction_handling"
  - "crypto_or_key_operation"

- D_external_system
  - "third_party_api_call"
  - "message_queue_operation"
  - "config_env_access"


## token length count

| Intent | Count | Min | Max | Median | Mean | Std |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| business_report_query | 1000 | 133 | 506 | 268 | 272.04 | 54.52 |
| cache_access | 1000 | 126 | 508 | 333 | 334.47 | 69.5 |
| command_execution | 1000 | 126 | 433 | 236 | 243.43 | 49.89 |
| config_change | 1000 | 233 | 507 | 387 | 388.26 | 65.64 |
| config_env_access | 1000 | 137 | 506 | 268 | 271.15 | 52.57 |
| crud_operation | 1000 | 198 | 510 | 439 | 431.19 | 66.41 |
| crypto_or_key_operation | 1000 | 152 | 507 | 366 | 376.9 | 77.64 |
| file_download | 1000 | 233 | 511 | 420 | 418.3 | 62.12 |
| file_upload | 1000 | 240 | 507 | 431 | 426.06 | 57.31 |
| filesystem_access | 1000 | 142 | 504 | 299.5 | 304.47 | 68.96 |
| internal_service_rpc_call | 1000 | 162 | 508 | 318.5 | 325.08 | 61.54 |
| message_queue_operation | 1000 | 177 | 512 | 323 | 331.7 | 68.35 |
| order_or_payment_operation | 1000 | 214 | 509 | 491 | 461.14 | 54.86 |
| orm_operation | 1000 | 126 | 509 | 279 | 289.82 | 75.95 |
| permission_check | 1000 | 135 | 507 | 305.5 | 312.59 | 76.45 |
| search_or_pagination | 1000 | 169 | 508 | 340 | 346.35 | 68.44 |
| sensitive_user_action | 1000 | 153 | 500 | 281 | 286.99 | 54.33 |
| sql_execution | 1000 | 91 | 504 | 187 | 191.01 | 48.38 |
| third_party_api_call | 1000 | 123 | 468 | 289 | 288.65 | 49.97 |
| token_or_session_handling | 1000 | 180 | 509 | 408.5 | 403.64 | 74.19 |
| transaction_handling | 1000 | 165 | 477 | 276 | 288.08 | 55.4 |
| user_login | 1000 | 144 | 506 | 344.5 | 352.62 | 84.77 |
| user_logout | 1000 | 164 | 507 | 326.5 | 330.27 | 61.32 |
| user_registration | 1000 | 210 | 508 | 372.5 | 376.39 | 64.83 |
| verification_sms_email_captcha | 1000 | 301 | 510 | 497 | 482.45 | 33.33 |
| workflow_or_status_update | 1000 | 220 | 508 | 413 | 411.9 | 64.78 |

# Training and test set counts per intent category

| Intent | Train | Test |
| :--- | :--- | :--- |
| **A: user_identity** | | |
| user_registration | 1000 | 191 |
| user_login | 1000 | 188 |
| user_logout | 1000 | 199 |
| permission_check | 1000 | 198 |
| token_or_session_handling | 1000 | 183 |
| verification_sms_email_captcha | 1000 | 99 |
| **B: core_business** | | |
| order_or_payment_operation | 1000 | 114 |
| file_upload | 1000 | 180 |
| file_download | 1000 | 176 |
| search_or_pagination | 1000 | 195 |
| config_change | 1000 | 189 |
| workflow_or_status_update | 1000 | 179 |
| crud_operation | 1000 | 172 |
| sensitive_user_action | 1000 | 199 |
| business_report_query | 1000 | 200 |
| **C: data_resource_access** | | |
| sql_execution | 1000 | 200 |
| orm_operation | 1000 | 198 |
| cache_access | 1000 | 198 |
| filesystem_access | 1000 | 198 |
| command_execution | 1000 | 200 |
| internal_service_rpc_call | 1000 | 198 |
| transaction_handling | 1000 | 200 |
| crypto_or_key_operation | 1000 | 176 |
| **D: external_system** | | |
| third_party_api_call | 1000 | 200 |
| message_queue_operation | 1000 | 200 |
| config_env_access | 1000 | 200 |
