# Archive Contents: Eviction Data Files (all_new_csv_xls_files.zip)

This archive (`all_new_csv_xls_files.zip`) contains key data files related to the eviction data processing and migration project. It includes the original uploaded spreadsheet, the cleaned versions of its various sheets, and the final migrated data for core entities.

## Archive Structure

The archive contains the following main directories and files at its root level after extraction:

1.  **`README.md`**: This file, providing an overview of the archive contents.

2.  **`all_new_files_for_user/`**: This is the main container directory within the zip.
    *   **`migrated_target_data/`**: Contains the structured CSV files representing the migrated data for core entities (Clients and Cases), along with detailed migration logs.
        *   `target_clients_v2.csv`: Initial migrated client data.
        *   `target_cases_v2_fuzzy_matched.csv`: Case data after initial fuzzy matching for ClientIDs.
        *   `target_cases_v3_auto_assigned.csv`: Case data after auto-assignment of high-confidence ClientIDs.
        *   `target_clients_v3_with_placeholders.csv`: The final client data, including any newly created placeholder clients.
        *   `target_cases_v4_placeholders_assigned.csv`: The final case data, with ClientIDs assigned (either matched or placeholder).
        *   `migration_log.txt`: Log from the initial migration stages.
        *   `migration_log_v2.txt`: Log from fuzzy matching stage.
        *   `migration_log_v3.txt`: Log from auto-assignment stage.
        *   `migration_log_v4.txt`: The latest migration log detailing placeholder creation and final ClientID assignments.

    *   **`cleaned_eviction_data/`**: Contains CSV files for each sheet from the original Excel spreadsheet after data cleaning and standardization.
        *   `all_evictions_files_cleaned.csv`
        *   `work_sheet_cleaned.csv`
        *   `final_invoices_cleaned.csv`
        *   `pm_info_cleaned.csv`
        *   `court_25_cleaned.csv`
        *   `court_24_cleaned.csv`
        *   `sheriff_evictions_cleaned.csv`
        *   `complaint_cleaned.csv`
        *   `summons_cleaned.csv`
        *   `alias_summons_cleaned.csv`
        *   `sps_alias_cleaned.csv`
        *   `aff_of_serv_cleaned.csv`
        *   `initial_invoice_cleaned.csv`
        *   `payment_plan_cleaned.csv`
        *   `outstanding_invoices_cleaned.csv`
        *   `new_invoice_list_cleaned.csv`
        *   `zoom_hearings_cleaned.csv`

    *   **`EVICTIONS 2025 NEW.xlsx`**: The original Excel spreadsheet provided for this project.

## Purpose of Files

*   **`EVICTIONS 2025 NEW.xlsx`**: The raw source data.
*   **`cleaned_eviction_data/`**: These files represent the state of the data after initial cleaning operations (standardizing formats, handling some inconsistencies). They are useful for understanding the source data quality and the transformations applied.
*   **`migrated_target_data/`**: These files, particularly `target_clients_v3_with_placeholders.csv` and `target_cases_v4_placeholders_assigned.csv`, represent the data mapped to the new target structure. The logs provide a detailed history of the migration steps, including ClientID matching and placeholder creation.

Please review the contents. If you have any questions, feel free to ask.
