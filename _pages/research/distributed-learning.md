```html
<style>
.fl-diagram {
  margin: 30px 0;
  padding: 28px;
  background: #f5f7fb;
  border: 1px solid #dce3ed;
  border-radius: 14px;
  color: #343b46;
  font-family: inherit;
}

.fl-diagram * {
  box-sizing: border-box;
}

.fl-diagram .diagram-title {
  text-align: center;
  font-size: 1.15em;
  font-weight: 700;
  margin-bottom: 22px;
}

.fl-diagram .server {
  max-width: 340px;
  margin: 0 auto;
  padding: 18px;
  text-align: center;
  background: #e2ebfa;
  border: 1px solid #9bb6e0;
  border-radius: 10px;
}

.fl-diagram .server strong,
.fl-diagram .client strong {
  display: block;
  margin-bottom: 6px;
}

.fl-diagram .server small,
.fl-diagram .client small {
  display: block;
  line-height: 1.5;
}

.fl-diagram .connections {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  text-align: center;
  color: #5276aa;
  font-size: 27px;
  line-height: 1.5;
}

.fl-diagram .clients {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 12px;
}

.fl-diagram .client {
  padding: 17px 10px;
  text-align: center;
  border-radius: 10px;
  border: 1px solid;
}

.fl-diagram .honest {
  background: #e8f5ec;
  border-color: #a5cfb2;
}

.fl-diagram .byzantine {
  background: #fff0ed;
  border-color: #e5b2aa;
}

.fl-diagram .honest strong {
  color: #286b43;
}

.fl-diagram .byzantine strong {
  color: #a33f34;
}

.fl-diagram .direction-label {
  text-align: center;
  color: #667085;
  font-size: 0.85em;
  margin: 10px 0 20px;
}

.fl-diagram .research-directions {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 14px;
  margin-top: 25px;
}

.fl-diagram .direction {
  padding: 17px;
  background: #fff;
  border: 1px solid #dce3ed;
  border-radius: 9px;
}

.fl-diagram .direction strong {
  display: block;
  color: #315b91;
  margin-bottom: 7px;
}

.fl-diagram .direction p {
  margin: 0;
  font-size: 0.9em;
  line-height: 1.6;
}

@media (max-width: 600px) {
  .fl-diagram {
    padding: 15px;
  }

  .fl-diagram .clients {
    gap: 6px;
  }

  .fl-diagram .client {
    padding: 12px 5px;
    font-size: 0.85em;
    overflow-wrap: anywhere;
  }

  .fl-diagram .research-directions {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="fl-diagram">

  <div class="diagram-title">
    Distributed and Federated Learning
  </div>

  <div class="server">
    <strong>Central Server</strong>
    <small>Model aggregation and global updates</small>
  </div>

  <div class="connections" aria-hidden="true">
    <div>↙</div>
    <div>↓</div>
    <div>↘</div>
  </div>

  <div class="clients">

    <div class="client honest">
      <strong>Client 1</strong>
      <small>Local data</small>
      <small>Honest update</small>
    </div>

    <div class="client honest">
      <strong>Client 2</strong>
      <small>Local data</small>
      <small>Honest update</small>
    </div>

    <div class="client byzantine">
      <strong>Client 3</strong>
      <small>Adversarial behavior</small>
      <small>Corrupted update</small>
    </div>

  </div>

  <div class="direction-label">
    Clients compute local updates; the server aggregates the contributions.
  </div>

  <div class="research-directions">

    <div class="direction">
      <strong>01 · Byzantine-Resilient Learning</strong>
      <p>
        Robust optimization and aggregation methods that mitigate
        malicious or corrupted client updates, including in
        heterogeneous federated learning.
      </p>
    </div>

    <div class="direction">
      <strong>02 · Adaptive Error Feedback</strong>
      <p>
        Communication-efficient optimization through adaptive
        compression and error feedback, reducing communication
        costs while preserving optimization accuracy.
      </p>
    </div>

  </div>

</div>
```
