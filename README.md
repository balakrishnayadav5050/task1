# task1
Summary of Data Cleaning Steps for Medical Appointment No Shows
I began by importing the dataset into a Pandas DataFrame.

I removed all duplicate rows to eliminate repeated records and ensure uniqueness.

I checked for missing values in the dataset to identify any incomplete entries.

Since this dataset had very few missing values, I handled them appropriately:

I filled missing values (if any) in categorical fields like Gender or Neighbourhood with "Unknown".

I corrected column names by converting them to lowercase and replacing spaces with underscores for cleaner syntax.

I standardized the Gender column by removing spaces and converting all values to uppercase (e.g., "f" → "F").

I made sure all date columns, such as ScheduledDay and AppointmentDay, were properly converted to datetime format.

I calculated the waiting time by subtracting the scheduled date from the appointment date and added it as a new column named waiting_days.

I verified and fixed data types: for example, ensuring Age was an integer and boolean columns like Diabetes were properly typed.

I checked for any negative or invalid age values (like Age < 0) and either corrected or removed them.

I standardized values in the No-show column by converting them to lowercase or renaming "No" to "Show" and "Yes" to "No-Show" for clarity.

I exported the cleaned dataset to a new CSV file named medical_appointments_cleaned.csv.
