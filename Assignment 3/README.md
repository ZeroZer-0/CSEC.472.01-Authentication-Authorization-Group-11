# README.md - CSEC 472 Assignment 3: Secure Authentication System

## Task 1 Implementation Reference

### Task 1-1-A: Implement Argon2 hashing to securely store user passwords
- Lines XX-XX: `init_password_hasher`
- Lines XX-XX: `register_user`

### Task 1-1-B: Store only the hashed version of the password in a JSON file
- Lines XX-XX: `register_user`

### Task 1-1-C: Use Argon2's salt and work factor to enhance security
- Lines XX-XX: `init_password_hasher`

### Task 1-2-A: Implement a login system that verifies user credentials securely
- Lines XX-XX: `login_user`

### Task 1-2-B: Password strength check
- Lines XX-XX: `check_password_quality`

### Task 1-2-C: Lock accounts for fifteen minutes after five failed login attempts
- Lines XX-XX: `check_lockout`
- Lines XX-XX: `fail_login`

### Task 1-2-D: Prevent timing attacks using constant-time password comparison
- Lines XX-XX: `verify_password`

### Task 1-3-A: Generate a six-digit TOTP based on HMAC(time, key)
- Lines 202-209: `generate_totp`

### Task 1-3-B: Store the TOTP with a one-minute expiration in a JSON file
- Lines 217-228: `simulate_authenticator`

### Task 1-3-C: Simulate an authenticator app by printing TOTP to console
- Lines 217-217: `simulate_authenticator`

### Task 1-3-D: Require users to enter the TOTP to complete login
- Lines 239-263: `verify_totp`
- Lines 265-294: `main`

### Task 1-4-A: Store user credentials in a JSON file securely
- Lines 99-106: `save_user_data`
- Lines 83-91: `load_user_data`

### Task 1-4-B: Securely erase memory used for plaintext passwords after verification
- Lines 133-139: `secure_erase`

### Task 1-4-C: Track hashed passwords, failed login attempts, OTPs, lockout time
- Lines 115-124: `initialize_user_record`

### Task 1-4-D: Ensure the database persists between program runs
- Lines 83-91: `load_user_data`
- Lines 99-106: `save_user_data`