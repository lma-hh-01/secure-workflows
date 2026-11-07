# secure-workflows

Zentrales Repository der „Plattform“ im Testbed zur Masterarbeit *Sicherheit in Software Supply Chains*.

Es enthält

- die wiederverwendbaren GitHub-Workflows, über die Anwendungs-Repositories ab Variante V1 bauen, signieren und attestieren (`.github/workflows/`),
- die Kyverno-Richtlinien, die an der Admission im Cluster und ab V3 bereits in der Pipeline geprüft werden (`policies/`).

Anwendungs-Repositories rufen die Workflows nur auf und können sie nicht verändern. Die Signatur stammt deshalb von der Identität dieser Workflows, und genau diese Identität prüft Kyverno.

Aufbau, Bedienung und Szenarien beschreibt das Repository [testbed](https://github.com/lma-hh-01/testbed).
