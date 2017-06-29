# How-to-OAuth2

# How to generate token?

1. Open PostMan, enter url = http://localhost:9999/oauth/token , select POST.
2. Under Authorization tab, Select Basic Auth
3. UserName = web_app, password = [empty]
4. Click UpdateRequest
5. Ensure header(2) have the following:
  a. Content-Type = application/x-www-form-urlencoded
  b. Authorization = Basic d2ViX2FwcDo=
6. In Body tab enter Grant_Type = password, username = admin, password=admin
7. Finally click Send button, response display below:

{
    "access_token": "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE0OTg3NjA3NDgsInVzZXJfbmFtZSI6ImFkbWluIiwiYXV0aG9yaXRpZXMiOlsiUk9MRV9BRE1JTiIsIlJPTEVfVVNFUiJdLCJqdGkiOiI3ODhhMjAwYy01MzA0LTQ0N2QtOTcwNy0wZGNlMmY1ODBjZDMiLCJjbGllbnRfaWQiOiJ3ZWJfYXBwIiwic2NvcGUiOlsib3BlbmlkIl19.HTavY-lrPXXOV0UrB_bJ0_490Hd6JoYtfJSgjRzHnepnUf_oRQqYZ84s-Ao6-NSGrMOnkZ4Wn2FxlqRhgGKW_TiCMJYKQEL84hPCXPWVVp9BRJn1eNFGWSP88ehubFO7BBjVFyDxwWDAtW13i6g_2qCza8M3WQadDxDVM-Be8Ko2amsx9y_Q0zzZjd15XgYp2nlNA_hzGjMhe8kNh2A7FGIAPP6wdzz867GxjGRS8SiZ3u8GqWrCEpcF-LbML3SPjIsgLQ0TgbLopy2EzHAIwGdjyuY3TLyrVILZlIOoEXvXdB88e2JpRXC3PRVepfpMxvPTbta_Ja_LxiV6x30anw",
    "token_type": "bearer",
    "refresh_token": "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX25hbWUiOiJhZG1pbiIsInNjb3BlIjpbIm9wZW5pZCJdLCJhdGkiOiI3ODhhMjAwYy01MzA0LTQ0N2QtOTcwNy0wZGNlMmY1ODBjZDMiLCJleHAiOjE1MDEzMDk1NDgsImF1dGhvcml0aWVzIjpbIlJPTEVfQURNSU4iLCJST0xFX1VTRVIiXSwianRpIjoiMTg4NTE1NzQtYjlhMi00MTgwLWI2ZDItOWQ2Y2VlNWM5ODVjIiwiY2xpZW50X2lkIjoid2ViX2FwcCJ9.NP95SMEdLvkjulI_KJ9AIem7JnwMbl1VsCPZgPttYVXKEsUCEDfhxRJ4XdeRTcovK2Fnbwteglils3Ikdv8seIpcVL5ia3eHUcqdtORQkbE8dgDoAl-KJfMU7GXTO58voJJ9tivDCYXUQbobXKHhpoETd7dIpSF3unNDRCib49ReVHr5M0Ldz4CtzkjjIru8wwDIP03Uk-QxdiZq-D9gem1ESW-REK57VCQXqZkyNAQygilZwvh2hqRSL2QuO_EHYuVU9_ZpXMu99IXOJqBQlLcKYWE2aeybanFj0y9amNmTfZujoQNXp3FCQNOEMXlchQ__GlQqqJj8Ct8Xie08iA",
    "expires_in": 43199,
    "scope": "openid",
    "jti": "788a200c-5304-447d-9707-0dce2f580cd3"
}
