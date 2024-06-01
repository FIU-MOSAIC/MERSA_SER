Device Data Export

The Devices category of your data export includes all of the Fitbit devices you have paired. This includes Devices.csv, Trackers.csv, Tracker Optional Configuration.csv, Scales.csv, and iOS App Notification Settings.csv

Files Included:
----------

Devices.csv

This is the list of all Devices you have paired.

    wire_id
    device_type
    serial_number
    enabled
    fw_version

----------

Trackers.csv

This is the configuration of all Trackers you have paired, which are the data tightly coupled with the physical device.

    tracker_id
    date_added
    last_sync_date_time
    batt_level
    hardware_rev
    is_display_distance
    is_display_calories
    is_display_clock
    is_display_flower
    is_display_elevation
    is_display_chatter
    is_right_handed
    tracker_name
    device_type
    on_dominant_hand
    is_display_active_minutes
    clock_face
    enable_ancs
    is_bonded
    is_display_steps
    alarm_update_time
    is_display_heart_rate
    heart_rate_tracking
    heart_rate_tracking_update_time
    tap_enabled
    tap_screen
    flick_enabled
    flick_screen

----------

Tracker Optional Configuration.csv

This is the additional configuration of all Trackers you have paired with various number of columns, which are optional and can be different between users.

    tracker_id
    enabled_notification_types
    on_right_hand
    clock_face
    enable_inactivity_alerts
    last_updated_last_ia_time
    last_reboot_time
    payments_enabled
    last_successful_wifi_connection_time
    last_successful_wifi_connectionipv4address
    last_successful_wifi_connectionipv6address
    last_successful_wifi_connectionssid
    live_data_disabled

----------

Scales.csv

This is the list of all Scales you have paired.

    scale_id
    short_name
    display_bf
    display_bf_mass_unit
    display_bmi
    user_icon_id


----------

iOS App Notification Settings.csv

This is the list of iOS applications that your Fitbit device can display notifications from. Notifications from apps with is_app_enabled “true” are displayed on the device, and apps with is_app_enabled “false” are not.

    user_id
    tracker_id
    mobile_app_name
    is_app_enabled
    show_partial_message
    is_default_message_app
    created_on
    modified_on
