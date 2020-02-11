## Getting Emails

        Usage:              rscript get_emails.R "regexp for matching outgoing email ids" max_emails
        Sample command:     rscript get_emails.R "russellgoldenberg" 999999
        Requires:           secret.json (see Russell)
        Output:             email_data.csv

On first use, the script will ask you to open browser window get permission for email id and password. The authorization will then be cached on the local machine for future use. Sometimes the script returns an error when the token expires. Rerun the script and it will work! If you have multiple address, you can pipe delimit (eg. `"russellgoldenberg|smokey"`).

## Exploratory Plots

        Usage:      rscript analysis.R
        Requires:   email_data.csv
        Output:     Rplots.pdf
