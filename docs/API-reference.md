# API Reference

This document describes the API endpoints for IEM-TestGen, a FastAPI web service that uses the GROQ large language model API to generate and manage test cases from plain-language requirements.

1. POST /generate-testcases
Description:
Generate test cases from a user-provided software requirement.

Request

Method: POST

URL: /generate-testcases

Content-Type: application/json

Body Example:

json
{
  "requirement_description": "The user should be able to reset their password via email."
}
Response

Status: 200 OK

Body Example:

json
{
  "testcases": [
    {
      "id": "TC001",
      "title": "Password Reset Email",
      "description": "Verify password reset can be initiated by email.",
      "steps": [
        "Navigate to login page",
        "Click 'Forgot Password'",
        "Enter email address",
        "Check email for reset link"
      ],
      "expected_result": "Password reset link sent to email.",
      "priority": "High",
      "status": "Open"
    }
    // ...more testcases
  ]
}

Possible Errors

400 Bad Request: Invalid input (e.g., missing "requirement_description").

500 Internal Server Error: GROQ API issue or unexpected error.