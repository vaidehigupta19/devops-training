# AWS S3 Bucket with Private Access

## Objective

Create an Amazon S3 bucket, enable Block Public Access, upload an image, and access it using the AWS CLI.

---

## Prerequisites

- AWS Account
- AWS CLI installed
- Git
- GitHub

---

## Steps Performed

### 1. Install AWS CLI

Verified the installation using:

```bash
aws --version
```

---

### 2. Login to AWS CLI

Authenticated using:

```bash
aws login
```

Configured the region:

```
ap-south-1
```

---

### 3. Create an S3 Bucket

Bucket Name:

```
vaidehi-s3-demo-2026
```

Region:

```
Asia Pacific (Mumbai) - ap-south-1
```

Enabled:

- Block Public Access
- ACLs Disabled

---

### 4. Upload an Image

Uploaded:

```
coding.jpeg
```

---

### 5. Verify Public Access

Opened the Object URL in a browser.

Result:

```
Access Denied
```

This confirms that the bucket is private.

---

### 6. List Buckets

```bash
aws s3 ls
```

Output:

```
2026-07-16 vaidehi-s3-demo-2026
```

---

### 7. Download the Image

```bash
aws s3 cp s3://vaidehi-s3-demo-2026/coding.jpeg .
```

Output:

```
download: s3://vaidehi-s3-demo-2026/coding.jpeg to .\coding.jpeg
```

---

## Commands Used

```bash
aws --version

aws login

aws s3 ls

aws s3 cp s3://vaidehi-s3-demo-2026/coding.jpeg .
```

---

## Screenshots

Include the following screenshots:

- AWS CLI Version
- S3 Bucket Created
- Block Public Access Enabled
- Image Uploaded Successfully
- Object Details
- Browser Showing "Access Denied"
- `aws login`
- `aws s3 ls`
- `aws s3 cp` Download Successful

---

## Outcome

- Successfully installed AWS CLI.
- Logged in to AWS CLI.
- Created a private Amazon S3 bucket.
- Uploaded an image.
- Verified that public access is blocked.
- Accessed the image securely using the AWS CLI.