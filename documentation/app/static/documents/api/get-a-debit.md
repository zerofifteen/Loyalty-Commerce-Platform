### Get a Debit

Retrieves the details of a previous debit. This retrieves a historical record of the debit transaction when it was created, including whether the transaction succeeded or failed. Requests must be signed with your app's credentials.

#### Parameters

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>lp-id</td>
            <td>The identifier of the loyalty program (LP).</td>
        </tr>
        <tr>
            <td>id</td>
            <td>The identifier of the debit.</td>
        </tr>
    </tbody>
</table>

#### Returns

The debit object if it exists, otherwise returns an [error](./?doc=reference-manual#errors).


