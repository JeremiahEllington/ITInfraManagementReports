# KPI Definitions (Concise)

| KPI | Definition | Formula Sketch | Source |
|-----|------------|----------------|--------|
| Availability% | Uptime vs total period | (TotalTime-DownTime)/TotalTime *100 | Monitoring APM |
| MTTR | Mean time to recover | Sum(ResolveTime-Start)/IncidentCount | Incident System |
| MTTA | Mean time to acknowledge | Sum(AckTime-Start)/IncidentCount | Incident System |
| IncidentCount | Count of production incidents | N | Incident System |
| Sev1Count | Critical incidents | Filter severity=1 | Incident System |
| ChangeSuccess% | Changes w/o incident | (SuccessChanges/TotalChanges)*100 | Change Mgmt |
| PatchCompliance% | Servers patched within window | Compliant/Total *100 | Patch Tool |
| VulnerabilityExposure | Outstanding high vulns | Count(CVSS>=7) | Scanner |
| BackupSuccess% | Completed / scheduled jobs | Success/Planned *100 | Backup System |
| RPO_Hours | Data loss exposure | Avg(LastBackupAgeHours) | Backup System |
| CapacityHeadroom% | Unused alloc vs capacity | (Capacity-Used)/Capacity*100 | Metrics Store |
| CostVariance% | (Actual-Budget)/Budget *100 | Derived | FinOps/Cost |