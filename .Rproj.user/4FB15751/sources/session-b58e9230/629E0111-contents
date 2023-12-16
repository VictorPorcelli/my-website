library(sendmailR)

# Retrieve form data
fname <- Sys.getenv("fname")
lname <- Sys.getenv("lname")
email <- Sys.getenv("email")
message <- Sys.getenv("message")

# Compose email
subject <- "New Contact Form Submission"
body <- paste("First Name:", fname, "\n",
              "Last Name:", lname, "\n",
              "Email:", email, "\n\n",
              "Message:", message)

# Set sender and recipient email addresses
from <- "victorjporcelli@gmail.com"
to <- "victorjporcelli@gmail.com"

# Set Gmail SMTP server details
smtp_server <- "smtp.gmail.com"
smtp_port <- 587  # Use the appropriate port for Gmail
smtp_user <- "victorjporcelli@gmail.com"
smtp_pass <- "soITgoes0808"  # Use an App Password for increased security

# Send email
sendmail(from, to, subject, body, control=list(smtpServer=smtp_server, 
                                               smtpPort = smtp_port,
                                               smtpUser=smtp_user,
                                               smtpPass=smtp_pass,
                                               ssl=FALSE))
