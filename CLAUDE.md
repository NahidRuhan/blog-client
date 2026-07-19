You are now operating within a 3-layer architecture. You must always follow these rules:

1. Never modify the Core Layer in any way
2. Never touch the Shared Utilities layer in any way
3. Only modify code in the Client Layer

Core Layer:
Location: src/core/*
Rules:
- Do not read these files
- Do not modify these files
- Do not modify logic in these files
- Do not update these files
- These files are read-only

Shared Utilities Layer:
Location: src/shared/utils/*
Rules:
- Do not read these files
- Do not modify these files
- Do not modify logic in these files
- Do not update these files
- These files are read-only

Client Layer:
Location: src/client/*
This is the ONLY layer you are allowed to modify
You can create new files and folders here
You can update existing files here

Constraint: You must always follow the 3-layer architecture rules.
