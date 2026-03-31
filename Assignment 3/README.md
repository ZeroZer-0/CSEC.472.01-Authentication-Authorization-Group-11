# README.md - CSEC 472 Assignment 3: Secure Authentication System

## Task 1 Implementation Reference

### Task 1-1-A: Implement Argon2 hashing to securely store user passwords
- Lines 92-93: `init_password_hasher`
- Lines 149-164: `register_user`

### Task 1-1-B: Store only the hashed version of the password in a JSON file
- Lines 165-80: `register_user`

### Task 1-1-C: Use Argon2's salt and work factor to enhance security
- Lines 92-93: `init_password_hasher`

### Task 1-2-A: Implement a login system that verifies user credentials securely
- Lines 190-208: `login_user`

### Task 1-2-B: Password strength check
- Lines 21-28: `check_password_quality`

### Task 1-2-C: Lock accounts for fifteen minutes after five failed login attempts
- Lines 57-74: `check_lockout`
- Lines 35-48: `fail_login`

### Task 1-2-D: Prevent timing attacks using constant-time password comparison
- Lines 83-87: `verify_password`

### Task 1-3-A: Generate a six-digit TOTP based on HMAC(time, key)
- Lines 218-225: `generate_totp`

### Task 1-3-B: Store the TOTP with a one-minute expiration in a JSON file
- Lines 233-244: `simulate_authenticator`

### Task 1-3-C: Simulate an authenticator app by printing TOTP to console
- Lines 233-244: `simulate_authenticator`

### Task 1-3-D: Require users to enter the TOTP to complete login
- Lines 255-279: `verify_totp`
- Lines 281-310: `main`

### Task 1-4-A: Store user credentials in a JSON file securely
- Lines 115-122: `save_user_data`
- Lines 99-107: `load_user_data`

### Task 1-4-B: Securely erase memory used for plaintext passwords after verification
- Lines 149-155: `secure_erase`

### Task 1-4-C: Track hashed passwords, failed login attempts, OTPs, lockout time
- Lines 131-140: `initialize_user_record`

### Task 1-4-D: Ensure the database persists between program runs
- Lines 115-122: `save_user_data`
- Lines 99-107: `load_user_data`