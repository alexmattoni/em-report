<script lang="ts">
    import type { PageData } from './$types';

    export let data: PageData;
</script>

<h1>EMS Report</h1>

<p> Input Patient Information</p>

<form>
<label for="ptfirstname"> Patient Name</label> <br>
<input type="text" id="ptfirstname"> <br>
<input type="text" id="ptlastname"> <br>

<label for="ptDOB"> DOB </label>
<input type="date" id = "ptDOB"> <br>

<label for="ptage"> Age</label>
<input type="number" id="ptage"> <br>

<!--  should save as 0 for male, 1 for female, 2 for unknown  -->
<label for="ptgender"> Gender</label>
<input type="number" id="ptgender"> <br>

<label for="pttype"> Patient Type</label>
<input type="text" id="pttype"> <br>

<label for="ptCC"> Chief Complaint</label>
<input type="text" id="ptCC"> <br>

<!-- implement dropdown later on -->
<label for="hospitaldestination"> Hospital Destination </label>
<input type="text" id="hospitaldestination"> <br>

<button id="notifyButton"> Notify </button>
</form>