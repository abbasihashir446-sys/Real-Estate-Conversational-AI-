# Final Verification

## Project
- Location: /mnt/data/real_estate_voice_agent_capstone
- Source files: 66

## Automated test result
```text
[32m.[0m[32m.[0m[32m.[0m[32m.[0m[33m                                                                     [100%][0m
[33m=============================== warnings summary ===============================[0m
tests/test_core.py::test_booking_duplicate_slot_rejected
  /mnt/data/real_estate_voice_agent_capstone/app/tools.py:43: DeprecationWarning: datetime.datetime.utcnow() is deprecated and scheduled for removal in a future version. Use timezone-aware objects to represent datetimes in UTC: datetime.datetime.now(datetime.UTC).
    row={"session_id":session_id, **payload, "logged_at":datetime.utcnow().isoformat()}

-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
[33m[32m4 passed[0m, [33m[1m1 warning[0m[33m in 0.83s[0m[0m

Spreadsheet runtime warmup failed during python startup
Traceback (most recent call last):
  File "/tmp/tmp.L2TH2Y5coc/artifact_tool_v2-2.8.22/artifact_tool/patches/warm_spreadsheet_runtime_on_startup.py", line 26, in warm_spreadsheet_runtime_on_startup
  File "/tmp/tmp.L2TH2Y5coc/artifact_tool_v2-2.8.22/artifact_tool/spreadsheet_warmup.py", line 785, in warm_spreadsheet_runtime
  File "/tmp/tmp.L2TH2Y5coc/artifact_tool_v2-2.8.22/artifact_tool/spreadsheet_warmup.py", line 720, in _warm_feature_flows
  File "/tmp/tmp.L2TH2Y5coc/artifact_tool_v2-2.8.22/artifact_tool/spreadsheet_warmup.py", line 704, in _warm_collaboration_flows
  File "/tmp/tmp.L2TH2Y5coc/artifact_tool_v2-2.8.22/artifact_tool/generated/interface/models.py", line 32317, in hydrate_crdt_from_proto
  File "/tmp/tmp.L2TH2Y5coc/artifact_tool_v2-2.8.22/artifact_tool/rpc/remote.py", line 749, in __call__
  File "/tmp/tmp.L2TH2Y5coc/artifact_tool_v2-2.8.22/artifact_tool/rpc/client.py", line 150, in call
artifact_tool.rpc.client.RemoteError: hydrateCrdtFromProto requires an empty collaborative document.
```

## Prepared evaluation outputs
- 20 RAG questions
- 20 RAG result rows
- 50 conversation test cases
- 10 security/injection tests
- metrics.csv
- demo_output.txt

## Scope
The implementation is a reproducible demo/reference architecture. External services such as telephony,
Fish Audio, Deepgram, Google Calendar, Gmail, PostgreSQL and a hosted vector database require credentials
and live adapters before production deployment.
