# dtllm-ir — reference implementation of a verifiable DT–LLM intermediate representation

| Module | Content | Paper |
|---|---|---|
| `schema/record.schema.json` | JSON Schema of a record | Table 12 |
| `ir_ref/bearing.py` | Characteristic frequencies | Eq. (1) |
| `ir_ref/facts.py` | Fact-extraction rules; each fact stores its inputs and rule parameters | Eqs. (2)–(4) |
| `ir_ref/providers.py` | **Interface to the digital twin** (`SignatureProvider`), file-based connector for an external DT (`FileDTProvider`), and a reference model | Section 3.7.3 |
| `ir_ref/dt_model.py` | Reference physics-based envelope model used by `ReferenceImpactModel` (not a DT) | — |
| `ir_ref/validate.py` | Schema validation, recomputation of every fact, validity-domain check | Table 12 |
| `ir_ref/checker.py` | Claim checker: identifiers, values, polarity, hypotheses stated as certainties, fault-type consistency | Section 3.7.3 |
| `examples/poc_cwru.py` | Example: complete chain applied to the public CWRU bearing data | Section 3.7.3 |



