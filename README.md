# Emergency dispatch quality assurance

A team project for software quality assurance at AUT. We developed and tested a c# emergency dispatch prototype, from requirements and design through to defect analysis and verification.

## Our process

1. **Define and review requirements.** Defined stakeholders, scope and functional and nonfunctional requirements. Resolved ambiguity and inconsistencies, then wrote measurable acceptance criteria.

2. **Design and build the prototype.** Applied SOLID principles, repository and strategy patterns, and dependency injection. Separated business rules, application services, database access and the web interface using Razor Pages and SQLite.

3. **Plan testing around risk.** Prioritised security, performance and reliability risks. Set the test scope and entry and exit criteria, and linked requirements to test cases through a traceability matrix.

4. **Design test cases.** Used equivalence partitioning, boundary value analysis, decision tables and state transitions. Covered expected behaviour, invalid input, unavailable resources and failure conditions.

5. **Execute and automate tests.** Combined manual workflow checks with MSTest unit, integration and HTTP tests. Checked concurrent assignments, recovery after restarts, access control, password hashing, data encryption and response times.

6. **Investigate and fix defects.** Tracked severity and priority in a defect register and investigated root causes using Five Whys. Fixed data loss, notification failures and test database isolation, then retested and added regression coverage.

7. **Add continuous integration.** Configured GitHub Actions to build the solution, run smoke tests and the full suite, and retain test reports.

8. **Evaluate the evidence.** Updated requirements as the implementation changed, compared results with acceptance criteria and documented remaining gaps in load testing, network security and access control coverage.

Read the [requirements and test plan](requirements-and-test-plan.pdf) and [implementation and verification report](implementation-and-verification-report.pdf) for the full process and evidence.

## Running locally

With the .NET 10 SDK installed:

```bash
dotnet run --project src/DispatchWeb
```

Open the URL shown in the terminal. Use the demo Admin account (`admin` / `admin-demo`) to explore all roles. This is a local demonstration, not a system for real emergency operations.

Run the tests from the repository root:

```bash
dotnet test Dispatch.slnx
```

## Contributors

<table>
  <tr>
    <td align="center" valign="top" width="1000">
      <br>
      <a href="https://github.com/LeoCaoProjects"><img src="https://github.com/LeoCaoProjects.png?size=160" width="72" height="72" alt="Leo Cao"></a>
      <p><a href="https://github.com/LeoCaoProjects"><strong>Leo Cao</strong></a></p>
      <br>
    </td>
    <td align="center" valign="top" width="1000">
      <br>
      <a href="https://github.com/fatehbhular"><img src="https://github.com/fatehbhular.png?size=160" width="72" height="72" alt="Fateh Bhular"></a>
      <p><a href="https://github.com/fatehbhular"><strong>Fateh Bhular</strong></a></p>
      <br>
    </td>
    <td align="center" valign="top" width="1000">
      <br>
      <a href="https://github.com/ShawnLeeyz"><img src="https://github.com/ShawnLeeyz.png?size=160" width="72" height="72" alt="Shawn Lee"></a>
      <p><a href="https://github.com/ShawnLeeyz"><strong>Shawn Lee</strong></a></p>
      <br>
    </td>
  </tr>
</table>
