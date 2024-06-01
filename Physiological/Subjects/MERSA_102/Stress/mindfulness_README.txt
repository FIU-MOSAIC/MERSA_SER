Mindfulness Data Export

The Mindfulness category of your data export includes all of the content you have added to Mindfulness in the app. This includes your mindfulness sessions logged  and your mindfulness goals.

Files Included:
----------

mindfulness_sessions.csv

This is the data related to mindfulness sessions.

   session_id                      - Unique id for the session logged
   activity_name                   - Name of the mindfulness activity (e.g. Meditation)
   average_heart_rate              - The user's average heart rate during session if backing HR data exists
   start_heart_rate                - The user's starting heart rate for the session if backing HR data exists
   end_heart_rate                  - The user's ending heart rate for the session if backing HR data exists
   duration                        - Duration in milliseconds of the content of the session
   start_date_time                 - Datetime of the start of the session
   end_date_time                   - Datetime of the end of the session
   session_type                    - Session type value if included when logging
   stress_metrics                  - Stress metrics map if included when logging
   pause_times                     - List of pause-unpause times (in seconds after session start) for a session

----------

mindfulness_eda_data_sessions.csv

This is the EDA data that was collected in the span for a session

   session_id                      - Unique id for the session logged
   timestamp                       - Timestamp for an EDA data point. First in the set corresponds to the timestamp and the rest are offset by 1, 2, 3, and 4 seconds.
   valid_data                      - Is data valid
   activation                      - Is activation true
   scl_avg                         - Average SCL recoded in time range

----------

mindfulness_goals.csv

These are the Mindfulness Goals set by the user
   date                            - Date on which goal was set
   days                            - Number of days set as mindfulness goal
   default_goal                    - Is this the default goal