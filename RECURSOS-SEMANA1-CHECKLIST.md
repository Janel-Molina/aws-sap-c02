# Checklist de Recursos — Semana 1 SAP-C02
**Dominio principal:** D1 — Organizational Complexity (26% del examen)
**Prioridad:** ALTA — resultado Assessment 0: **40%** (debilidad crítica)
**Fecha de inicio real:** 16 octubre 2026 (Día 0 completado)

---

## 📁 Documentación oficial — Estado

| # | Archivo | Tamaño | Estado | Prioridad S1 |
|---|---------|--------|--------|--------------|
| 1 | `Guía de examen (SAP-C02).pdf` | 637 KB | ✅ Presente | 🔴 LEER PRIMERO |
| 2 | `aws-organizations-best-practices.pdf` | 1.8 MB | ✅ Descargado hoy | 🔴 ESENCIAL S1 |
| 3 | `wellarchitected-framework.pdf` | 11 MB | ✅ Presente | 🟡 Referencia general |
| 4 | `wellarchitected-security-pillar.pdf` | 2.8 MB | ✅ Descargado hoy | 🟡 S2-S3 (Security) |

---

## 📌 Links de referencia clave

### Documentación oficial AWS (online)
- 🔗 [Guía de examen SAP-C02 oficial](https://d1.awsstatic.com/training-and-certification/docs-sa-pro/AWS-Certified-Solutions-Architect-Professional_Exam-Guide.pdf)
- 🔗 [AWS Organizations — Documentación](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_introduction.html)
- 🔗 [Service Control Policies (SCPs)](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps.html)
- 🔗 [AWS Control Tower](https://docs.aws.amazon.com/controltower/latest/userguide/what-is-control-tower.html)
- 🔗 [AWS IAM Identity Center (SSO)](https://docs.aws.amazon.com/singlesignon/latest/userguide/what-is.html)
- 🔗 [AWS RAM (Resource Access Manager)](https://docs.aws.amazon.com/ram/latest/userguide/what-is.html)
- 🔗 [Transit Gateway](https://docs.aws.amazon.com/vpc/latest/tgw/what-is-transit-gateway.html)
- 🔗 [VPC Peering](https://docs.aws.amazon.com/vpc/latest/peering/what-is-vpc-peering.html)
- 🔗 [AWS Direct Connect](https://docs.aws.amazon.com/directconnect/latest/UserGuide/Welcome.html)

### Whitepapers prioritarios descargados
- 📄 `aws-organizations-best-practices.pdf` → Whitepaper: *Organizing Your AWS Environment Using Multiple Accounts*
- 📄 `wellarchitected-security-pillar.pdf` → AWS Well-Architected Security Pillar (para S2/S3)

---

## 📅 Plan de la Semana 1 — Dominio 1: Organizational Complexity

### Objetivo de la semana
> Subir D1 de **40% → ≥65%** entendiendo el gobierno multi-cuenta en AWS.

### Temas a cubrir (en orden)

#### Bloque 1 — Fundamentos (Días 1-2)
- [ ] **AWS Organizations**: OUs, SCPs, políticas de etiquetado, billing consolidado
- [ ] **Multi-account strategy**: Landing Zone, account vending
- [ ] **AWS Control Tower**: guardrails preventivos vs detectivos
- [ ] **Leer:** Guía de examen SAP-C02 (sección D1 completa)
- [ ] **Leer:** `aws-organizations-best-practices.pdf` (capítulos 1-4)

#### Bloque 2 — Identidad y Acceso Federado (Días 2-3)
- [ ] **IAM Identity Center (SSO)**: permission sets, attribute-based access
- [ ] **AWS RAM**: compartir recursos entre cuentas sin VPC peering
- [ ] **STS AssumeRole**: cross-account roles, trust policies
- [ ] **SCPs vs IAM Policies**: diferencias, casos de uso, limitaciones

#### Bloque 3 — Networking Multi-cuenta (Días 3-4)
- [ ] **Transit Gateway**: conectar múltiples VPCs y on-premises
- [ ] **VPC Peering vs Transit Gateway**: cuándo usar cada uno
- [ ] **AWS Direct Connect**: conexión dedicada, Virtual Interfaces
- [ ] **VPN Site-to-Site vs Direct Connect**: trade-offs de costo y latencia

#### Bloque 4 — Gobierno y Compliance (Días 4-5)
- [ ] **AWS Config**: reglas, conformance packs, aggregators multi-cuenta
- [ ] **AWS CloudTrail Organizations**: trail organizacional
- [ ] **AWS Security Hub**: agregación de findings multi-cuenta
- [ ] **AWS GuardDuty Organizations**: threat detection centralizado

#### Bloque 5 — Labs y Preguntas (Días 5-7)
- [ ] Lab: Crear OU y SCP restrictiva en el lab account
- [ ] Lab: Crear cross-account role y asumir desde CLI
- [ ] 30 preguntas de práctica D1 con análisis de errores
- [ ] Registrar errores en `/aws-sap-c02/mistakes/`

---

## 🎯 Métricas objetivo Semana 1

| Métrica | Objetivo |
|---------|---------|
| Horas estudiadas | 15-20h |
| Preguntas D1 | ≥30 |
| Accuracy D1 | ≥65% |
| Labs completados | ≥2 |
| Architecture drills | ≥3 |

---

## 📊 Estado del entorno de laboratorio

| Recurso | Estado |
|---------|--------|
| Stack CloudFormation `sap-c02-lab` | ✅ Desplegado (us-east-1) |
| VPC con subnets públicas/privadas | ✅ Activo |
| Security Groups (EC2, RDS, ALB) | ✅ Configurados |
| NAT Gateway | ❌ Deshabilitado ($0 cost) |
| Repositorio GitHub | ✅ https://github.com/Janel-Molina/aws-sap-c02 |

---

## 📝 Notas del Assessment 0 (Día 0 — 16 oct 2026)

Resultados:
- D1 (Organizational Complexity): **40%** ← Debilidad crítica
- D2 (New Solutions): **80%**
- D3 (Continuous Improvement): **60%**
- D4 (Migration & Modernization): **60%**
- **Total: 60%** (estimado real ~25% sin deducción)

Observación: Las preguntas del Assessment 0 eran predecibles. El nivel real del examen SAP-C02 será significativamente más difícil (escenarios largos con múltiples restricciones).

---

## 🔮 Recursos para semanas posteriores (NO para S1)

| Recurso | Semana sugerida | Link |
|---------|----------------|------|
| Well-Architected Security Pillar (descargado) | S2-S3 | `wellarchitected-security-pillar.pdf` |
| Well-Architected Framework completo (descargado) | Referencia | `wellarchitected-framework.pdf` |
| AWS re:Invent sessions D1 (YouTube) | S1-S2 | Buscar: "AWS Organizations best practices re:Invent" |
| AWS Migration whitepaper | S7-S8 | https://docs.aws.amazon.com/pdfs/whitepapers/latest/aws-migration-whitepaper/aws-migration-whitepaper.pdf |
| Serverless Application Lens | S4-S5 | https://docs.aws.amazon.com/pdfs/wellarchitected/latest/serverless-applications-lens/wellarchitected-serverless-applications-lens.pdf |

---

*Última actualización: 2026-10-16 | Generado por Claude durante Día 0*
