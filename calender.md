'''
import calendar
def display_calendar(year, month):
    """Displays a calendar for the specified year and month."""
    # Create a calendar object
    cal = calendar.monthcalendar(year, month)

    # Print the calendar header
    print(calendar.month_name[month], year)
    print("Mo Tu We Th Fr Sa Su")

    # Print each week of the calendar
    for week in cal:
        for day in week:
            # Print each day of the week, or a blank space if the day is 0
            if day > 0:
                print(f"{day:2d}", end=" ")
            else:
                print("  ", end=" ")
        print()
		
# Get the year and month from the user
year = int(input("Enter the year: "))
month = int(input("Enter the month (1-12): "))

# Call the function to display the calendar
display_calendar(year, month)
'''