---
title: "Improving Public Health with Action and Better Policies"
description: "Our latest survey: Health & Wellness"
featured_image: "/images/health-and-wellness-background-image.png"

sections:
  - type: "report"
    heading: "Our Latest Report"
    subheading: "Health & Wellness Survey Results"
    metrics:
      - title: "Health Policy Survey"
        description: "A comprehensive survey on public health preferences across all U.S. states."
        cta: "View Full Results"
        cta_link: "#"
      - bullets:
          - title: "Participants"
            value: "20,000+"
            icon: "/icons/people.svg"
          - title: "States Covered"
            value: "30"
            icon: "/icons/flag.svg"
    key_findings:
      - title: "Key Findings"
      - list:
        - "**_80% of adults_** nationwide support policies that ensure affordable healthcare for all."
        - "**Broad bipartisan support** exists for expanding mental health services."
        - "**Regional preferences** reflect varying needs, with urban areas prioritizing preventive care and rural areas focusing on emergency services."
  - type: "about"
    heading: "About"
    subheading: "We are dedicated to fostering environmental sustainability for a healthier planet."
    what_we_do:
      title: "We empower communities to take action for a greener future:"
      bullets:
        - "You share your concerns and ideas about the most pressing environmental challenges."
        - "We connect individuals and groups working on local environmental solutions."
        - "Together, we organize campaigns, cleanups, and sustainability projects that make a real impact."
        - "When enough people get involved, we create change from the ground up, inspiring others to take action."

---

{{< code-tabs >}}

```go-html-template {linenos=inline hl_lines=[3]}
{{ range .Pages }}

{{ .Title }}
{{ .Description }}

{{ end }}
```

```python {linenos=inline hl_lines=[3,"6-8"] style=monokai}
from qdrant_client.models import PointStruct

operation_info = client.upsert(
    collection_name="test_collection",
    wait=True,
    points=[
        PointStruct(id=1, vector=[0.05, 0.61, 0.76, 0.74], payload={"city": "Berlin"}),
        PointStruct(id=2, vector=[0.19, 0.81, 0.75, 0.11], payload={"city": "London"}),
        PointStruct(id=3, vector=[0.36, 0.55, 0.47, 0.94], payload={"city": "Moscow"}),
        PointStruct(id=4, vector=[0.18, 0.01, 0.85, 0.80], payload={"city": "New York"}),
        PointStruct(id=5, vector=[0.24, 0.18, 0.22, 0.44], payload={"city": "Beijing"}),
        PointStruct(id=6, vector=[0.35, 0.08, 0.11, 0.44], payload={"city": "Mumbai"}),
    ],
)

print(operation_info)
```
```typescript
const operationInfo = await client.upsert("test_collection", {
  wait: true,
  points: [
    { id: 1, vector: [0.05, 0.61, 0.76, 0.74], payload: { city: "Berlin" } },
    { id: 2, vector: [0.19, 0.81, 0.75, 0.11], payload: { city: "London" } },
    { id: 3, vector: [0.36, 0.55, 0.47, 0.94], payload: { city: "Moscow" } },
    { id: 4, vector: [0.18, 0.01, 0.85, 0.80], payload: { city: "New York" } },
    { id: 5, vector: [0.24, 0.18, 0.22, 0.44], payload: { city: "Beijing" } },
    { id: 6, vector: [0.35, 0.08, 0.11, 0.44], payload: { city: "Mumbai" } },
  ],
});

console.debug(operationInfo);

```
```rust
use qdrant_client::qdrant::{PointStruct, UpsertPointsBuilder};

let points = vec![
    PointStruct::new(1, vec![0.05, 0.61, 0.76, 0.74], [("city", "Berlin".into())]),
    PointStruct::new(2, vec![0.19, 0.81, 0.75, 0.11], [("city", "London".into())]),
    PointStruct::new(3, vec![0.36, 0.55, 0.47, 0.94], [("city", "Moscow".into())]),
    // ..truncated
];

let response = client
    .upsert_points(UpsertPointsBuilder::new("test_collection", points).wait(true))
    .await?;

dbg!(response);
```
{{</ code-tabs >}}


## Project Summary: "Improving Public Health with Better Policies"

This project focuses on raising awareness and advocating for better public health policies through comprehensive surveys and citizen engagement. The project features a series of surveys that assess public opinion on key health issues across the United States, including access to affordable healthcare, mental health services, and regional healthcare needs. The initiative, led by **HealthyGov**, aims to empower individuals to advocate for policies that will improve health outcomes for all, regardless of socioeconomic background.

The project highlights key survey findings, such as broad bipartisan support for healthcare reform, and offers citizens opportunities to participate in shaping health policy through email and cell phone updates. HealthyGov encourages people to stay informed about policy changes and contribute to a collective effort to influence lawmakers. This initiative supports the idea that when enough voices unite, lawmakers will take action.


{{< code-tabs >}}
```go {linenos=inline hl_lines=[3,"6-8"] style=dark}
package main

import "fmt"

func main() {
    for i := 0; i < 3; i++ {
        fmt.Println("Value of i:", i)
    }
}
```
```python
print("Hello Python!")
print("Hello Python!")
print("Hello Python!")
print("Hello Python!")
```
```rust
echo "Hello Bash"
```
{{</ code-tabs >}}

## Key Components:
- **Health Policy Survey**: A nationwide survey on public health preferences and key issues.
- **Key Findings**: Insights on public support for affordable healthcare, mental health services, and regional healthcare needs.
- **Engagement Opportunities**: Invitations for users to join the movement by submitting their email or phone number for updates and policy news.

This project combines data-driven insights with grassroots activism to push for impactful, widely supported changes in U.S. healthcare policy.


