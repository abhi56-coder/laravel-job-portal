# Database Schema Plan

## users

- id
- name
- email
- password
- role: admin, candidate, employer
- created_at
- updated_at

## candidate_profiles

- id
- user_id
- phone
- location
- experience_years
- current_ctc
- expected_ctc
- skills
- summary
- created_at
- updated_at

## employer_profiles

- id
- user_id
- company_name
- company_website
- industry
- location
- description
- created_at
- updated_at

## jobs

- id
- employer_id
- title
- description
- location
- salary_min
- salary_max
- experience_required
- skills_required
- status: pending, approved, closed
- created_at
- updated_at

## job_applications

- id
- job_id
- candidate_id
- resume_id
- cover_note
- status: applied, shortlisted, rejected, selected
- created_at
- updated_at

## resumes

- id
- candidate_id
- file_name
- file_path
- created_at
- updated_at

## saved_jobs

- id
- candidate_id
- job_id
- created_at
