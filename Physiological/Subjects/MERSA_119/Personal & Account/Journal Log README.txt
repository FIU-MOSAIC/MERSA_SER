Journal Logging Data Export

The Journal Logging category of your export includes all of the content you have added to the covid survey, temperature and symptom logging if you have opted in. This includes journal entries, survey in progress, and survey responses
Files Included:
----------

journal_entries.csv

This is the journal entry related to temperature and symptoms

    entry_id                          - Internal id of the journal entry
    log_time                          - Date at which the entry was logged
    log_type                          - The type of journal entry logged, for example: temperature, runny_nose
    value                             - Internal numerical value to represent degree of journal entry
    meta                              - Meta data that includes information such as temperature units
    entry_category                    - Category to which the log_type belongs to
    zone_offset                       - Zone offset when the entry was logged

----------

covid_survey.csv

This is the survey meta data for a survey in progress

    survey_id                         - Internal id for the survey
    log_time                          - Date at which the survey was logged
    zone_offset                       - Zone offset when the survey in progress was submitted
    survey_status                     - Completed or in progress

----------

covid_survey_response.csv

This is the survey response related data

    survey_id                         - Internal id for the survey
    response_id                       - Internal id for survey response
    log_time                          - Date at which the survey response was logged
    zone_offset                       - Zone offset when the survey response was submitted
    question_key                      - Key name of the current question
    response                          - Survey response text
