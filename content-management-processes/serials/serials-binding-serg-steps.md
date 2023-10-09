# Serials Binding (SERG steps)

{% hint style="info" %}
This is part of the overall [Serials Binding](../../reference/workflow-overviews/serials-binding-overview.md) workflow
{% endhint %}

### Step 7: Update holding records <a href="#docs-internal-guid-824b8999-7fff-4947-5378-1e57dfa512b4" id="docs-internal-guid-824b8999-7fff-4947-5378-1e57dfa512b4"></a>

When Serials & E-Resources Assistant receives binding slips from Monograph Acquisitions:

* Add/update 866 fields in the original holding record and the wrlc holding record based on the items in each location
* Remove any legacy or unnecessary notes from the 852 holding field, for example: "All bound volumes located off site (WRLC Center). To retrieve, please submit a Consortium Loan Request form. Bound volumes are Library Use Only."

<figure><img src="../../.gitbook/assets/image (12).png" alt="A holding record with a subfield z of All bound volumes located off site (WRLC Center). To retrieve, please submit a Consortium Loan Request form. Bound volumes are Library Use Only."><figcaption><p>Example of legacy note from Voyager. The $z is no longer needed in our Alma environment.</p></figcaption></figure>

* Discard the slip
