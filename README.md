<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Las Lomas Karolina</title>
    <!-- Tailwind CSS CDN for styling -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom font for a clean look */
        body {
            font-family: 'Inter', sans-serif;
        }
    </style>
</head>
<body class="bg-gray-100 flex items-center justify-center p-4 md:p-8">
    <div class="bg-white p-6 rounded-xl shadow-2xl w-full max-w-3xl mx-auto">
        <h1 class="text-3xl font-bold text-center text-gray-800 mb-4 md:mb-6">Las Lomas Karolina</h1>
        <p class="text-center text-gray-600 mb-6 md:mb-8 text-sm md:text-base">
            In accordance with current registration regulations in Spain, we kindly request that you provide the following details for all guests booking the apartment.
        </p>

        <!-- The main form -->
        <form id="userDataForm" class="space-y-6">
            <div id="guests-container" class="space-y-8">
                <!-- Guest Form 1 (This will be the template) -->
                <div class="guest-form bg-gray-50 p-6 rounded-lg border border-gray-200">
                    <div class="flex justify-between items-center mb-4">
                        <h2 class="text-xl font-bold text-gray-800">Guest 1</h2>
                    </div>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <div>
                            <label for="name-1" class="block text-sm font-medium text-gray-700">Name</label>
                            <input type="text" id="name-1" name="name" required
                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                        </div>
                        <div>
                            <label for="firstSurname-1" class="block text-sm font-medium text-gray-700">First Surname</label>
                            <input type="text" id="firstSurname-1" name="firstSurname" required
                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                        </div>
                        <div>
                            <label for="secondSurname-1" class="block text-sm font-medium text-gray-700">Second Surname</label>
                            <input type="text" id="secondSurname-1" name="secondSurname"
                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                        </div>
                        <div>
                            <label for="birthdate-1" class="block text-sm font-medium text-gray-700">Birthdate</label>
                            <input type="date" id="birthdate-1" name="birthdate" required
                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                        </div>
                        <div>
                            <label for="emailAddress-1" class="block text-sm font-medium text-gray-700">Email Address</label>
                            <input type="email" id="emailAddress-1" name="emailAddress" required
                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                        </div>
                        <div>
                            <label for="telephoneNumber-1" class="block text-sm font-medium text-gray-700">Telephone Number</label>
                            <input type="tel" id="telephoneNumber-1" name="telephoneNumber" required
                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                        </div>
                        <div>
                            <label for="identificationType-1" class="block text-sm font-medium text-gray-700">Type of identification document</label>
                            <select id="identificationType-1" name="identificationType" required
                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                <option value="" disabled selected>Select one...</option>
                                <option value="NIE">NIE</option>
                                <option value="NIF">NIF</option>
                                <option value="ID card">ID card</option>
                                <option value="Passport">Passport</option>
                            </select>
                        </div>
                        <div>
                            <label for="documentNumber-1" class="block text-sm font-medium text-gray-700">Document Number</label>
                            <input type="text" id="documentNumber-1" name="documentNumber" required
                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                        </div>
                        <div class="col-span-1 md:col-span-2 hidden" id="documentSupportContainer-1">
                            <label for="documentSupport-1" class="block text-sm font-medium text-gray-700">SOPORTE DEL DOCUMENTO</label>
                            <input type="text" id="documentSupport-1" name="documentSupport"
                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                        </div>
                    </div>
                    
                    <div class="residential-address-section mt-6 pt-6 border-t border-gray-300">
                        <h2 class="text-xl font-bold text-gray-800 mb-4">Residential Address</h2>
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                            <div>
                                <label for="street-1" class="block text-sm font-medium text-gray-700">Street</label>
                                <input type="text" id="street-1" name="street" required
                                    class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                            </div>
                            <div>
                                <label for="streetNumber-1" class="block text-sm font-medium text-gray-700">Street Number</label>
                                <input type="text" id="streetNumber-1" name="streetNumber" required
                                    class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                            </div>
                            <div>
                                <label for="town-1" class="block text-sm font-medium text-gray-700">Town</label>
                                <input type="text" id="town-1" name="town" required
                                    class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                            </div>
                            <div>
                                <label for="postalCode-1" class="block text-sm font-medium text-gray-700">Postal Code</label>
                                <input type="text" id="postalCode-1" name="postalCode" required
                                    class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                            </div>
                            <div>
                                <label for="province-1" class="block text-sm font-medium text-gray-700">Province</label>
                                <input type="text" id="province-1" name="province"
                                    class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                            </div>
                            <div>
                                <label for="country-1" class="block text-sm font-medium text-gray-700">Country</label>
                                <input type="text" id="country-1" name="country" required
                                    class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- New checkbox to copy address -->
            <div class="flex items-center space-x-2 pt-4">
                <input type="checkbox" id="copyAddressCheckbox"
                       class="h-4 w-4 text-indigo-600 border-gray-300 rounded focus:ring-indigo-500">
                <label for="copyAddressCheckbox" class="text-sm font-medium text-gray-700 cursor-pointer">
                    Residential Address is the same for all guests
                </label>
            </div>

            <!-- Add Guest Button -->
            <button type="button" id="addGuestBtn"
                    class="w-full flex justify-center py-3 px-4 rounded-md shadow-sm text-sm font-medium text-indigo-600 bg-indigo-100 hover:bg-indigo-200 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500 transition duration-150 ease-in-out">
                Add Another Guest
            </button>

            <!-- Submit Button -->
            <button type="submit" id="generateBtn"
                    class="w-full flex justify-center py-3 px-4 rounded-md shadow-sm text-sm font-medium text-white bg-indigo-600 hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500 transition duration-150 ease-in-out">
                Check in
            </button>
        </form>

        <!-- Area to display the generated XML string -->
        <div id="xmlOutputContainer" class="mt-8 hidden">
            <h2 class="text-xl font-bold text-gray-800 mb-2">Generated XML</h2>
            <p class="text-gray-600 text-sm mb-4">
                Click the "Download XML" button to save the file, then upload it to your Google Drive.
            </p>
            <textarea id="xmlOutput" rows="10" readonly
                      class="block w-full p-4 border border-gray-300 rounded-md bg-gray-50 text-gray-700 font-mono resize-none text-sm"></textarea>
            <div class="mt-4 flex flex-col md:flex-row justify-center space-y-2 md:space-y-0 md:space-x-4">
                <button id="downloadBtn"
                        class="inline-flex items-center justify-center px-4 py-2 border border-transparent text-sm font-medium rounded-md shadow-sm text-white bg-blue-600 hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-500 transition duration-150 ease-in-out">
                    <svg class="-ml-1 mr-2 h-5 w-5" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor">
                        <path d="M10 2a.75.75 0 01.75.75v8.5a.75.75 0 01-1.5 0V2.75A.75.75 0 0110 2z" />
                        <path fill-rule="evenodd" d="M5.25 12a.75.75 0 01.75-.75h8a.75.75 0 010 1.5h-8a.75.75 0 01-.75-.75zm0 3a.75.75 0 01.75-.75h8a.75.75 0 010 1.5h-8a.75.75 0 01-.75-.75zM4.75 12a.75.75 0 00-.75.75v.5c0 .414.336.75.75.75h10.5a.75.75 0 00.75-.75v-.5a.75.75 0 00-.75-.75H4.75zM4.75 15a.75.75 0 00-.75.75v.5a.75.75 0 00.75.75h10.5a.75.75 0 00.75-.75v-.5a.75.75 0 00-.75-.75H4.75z" clip-rule="evenodd" />
                    </svg>
                    Download XML
                </button>
            </div>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Get references to the main elements
            var form = document.getElementById('userDataForm');
            var guestsContainer = document.getElementById('guests-container');
            var addGuestBtn = document.getElementById('addGuestBtn');
            var copyAddressCheckbox = document.getElementById('copyAddressCheckbox');
            var xmlOutputContainer = document.getElementById('xmlOutputContainer');
            var xmlOutput = document.getElementById('xmlOutput');
            var downloadBtn = document.getElementById('downloadBtn');

            var guestCount = 1;

            // Function to create a new guest form section
            function createGuestForm(guestNumber) {
                var newGuestForm = document.createElement('div');
                newGuestForm.classList.add('guest-form', 'bg-gray-50', 'p-6', 'rounded-lg', 'border', 'border-gray-200', 'mt-8');

                var headerHtml = `<div class="flex justify-between items-center mb-4">
                                     <h2 class="text-xl font-bold text-gray-800">Guest ${guestNumber}</h2>
                                     <button type="button" class="remove-guest-btn text-red-500 hover:text-red-700 transition duration-150 ease-in-out">
                                         <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                                             <path stroke-linecap="round" stroke-linejoin="round" d="M19 7l-.867 12.142A2 2 0 0116.035 21H7.965a2 2 0 01-1.995-1.858L5 7m5 4v6m4-6v6m1-10V4a1 1 0 00-1-1h-4a1 1 0 00-1 1v3M4 7h16" />
                                         </svg>
                                     </button>
                                 </div>`;
                var formHtml = `<div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                    <div>
                                        <label for="name-${guestNumber}" class="block text-sm font-medium text-gray-700">Name</label>
                                        <input type="text" id="name-${guestNumber}" name="name" required
                                            class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                    </div>
                                    <div>
                                        <label for="firstSurname-${guestNumber}" class="block text-sm font-medium text-gray-700">First Surname</label>
                                        <input type="text" id="firstSurname-${guestNumber}" name="firstSurname" required
                                            class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                    </div>
                                    <div>
                                        <label for="secondSurname-${guestNumber}" class="block text-sm font-medium text-gray-700">Second Surname</label>
                                        <input type="text" id="secondSurname-${guestNumber}" name="secondSurname"
                                            class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                    </div>
                                    <div>
                                        <label for="birthdate-${guestNumber}" class="block text-sm font-medium text-gray-700">Birthdate</label>
                                        <input type="date" id="birthdate-${guestNumber}" name="birthdate" required
                                            class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                    </div>
                                    <div>
                                        <label for="emailAddress-${guestNumber}" class="block text-sm font-medium text-gray-700">Email Address</label>
                                        <input type="email" id="emailAddress-${guestNumber}" name="emailAddress" required
                                            class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                    </div>
                                    <div>
                                        <label for="telephoneNumber-${guestNumber}" class="block text-sm font-medium text-gray-700">Telephone Number</label>
                                        <input type="tel" id="telephoneNumber-${guestNumber}" name="telephoneNumber" required
                                            class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                    </div>
                                    <div>
                                        <label for="identificationType-${guestNumber}" class="block text-sm font-medium text-gray-700">Type of identification document</label>
                                        <select id="identificationType-${guestNumber}" name="identificationType" required
                                            class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                            <option value="" disabled selected>Select one...</option>
                                            <option value="NIE">NIE</option>
                                            <option value="NIF">NIF</option>
                                            <option value="ID card">ID card</option>
                                            <option value="Passport">Passport</option>
                                        </select>
                                    </div>
                                    <div>
                                        <label for="documentNumber-${guestNumber}" class="block text-sm font-medium text-gray-700">Document Number</label>
                                        <input type="text" id="documentNumber-${guestNumber}" name="documentNumber" required
                                            class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                    </div>
                                    <div class="col-span-1 md:col-span-2 hidden" id="documentSupportContainer-${guestNumber}">
                                        <label for="documentSupport-${guestNumber}" class="block text-sm font-medium text-gray-700">SOPORTE DEL DOCUMENTO</label>
                                        <input type="text" id="documentSupport-${guestNumber}" name="documentSupport"
                                            class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                    </div>
                                </div>
                                
                                <div class="residential-address-section mt-6 pt-6 border-t border-gray-300">
                                    <h2 class="text-xl font-bold text-gray-800 mb-4">Residential Address</h2>
                                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                        <div>
                                            <label for="street-${guestNumber}" class="block text-sm font-medium text-gray-700">Street</label>
                                            <input type="text" id="street-${guestNumber}" name="street" required
                                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                        </div>
                                        <div>
                                            <label for="streetNumber-${guestNumber}" class="block text-sm font-medium text-gray-700">Street Number</label>
                                            <input type="text" id="streetNumber-${guestNumber}" name="streetNumber" required
                                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                        </div>
                                        <div>
                                            <label for="town-${guestNumber}" class="block text-sm font-medium text-gray-700">Town</label>
                                            <input type="text" id="town-${guestNumber}" name="town" required
                                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                        </div>
                                        <div>
                                            <label for="postalCode-${guestNumber}" class="block text-sm font-medium text-gray-700">Postal Code</label>
                                            <input type="text" id="postalCode-${guestNumber}" name="postalCode" required
                                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                        </div>
                                        <div>
                                            <label for="province-${guestNumber}" class="block text-sm font-medium text-gray-700">Province</label>
                                            <input type="text" id="province-${guestNumber}" name="province"
                                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                        </div>
                                        <div>
                                            <label for="country-${guestNumber}" class="block text-sm font-medium text-gray-700">Country</label>
                                            <input type="text" id="country-${guestNumber}" name="country" required
                                                class="mt-1 block w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500 transition duration-150 ease-in-out text-sm">
                                        </div>
                                    </div>
                                </div>
                `;

                if (guestNumber > 1) {
                     newGuestForm.innerHTML = headerHtml + formHtml;
                } else {
                     newGuestForm.innerHTML = `<h2 class="text-xl font-bold text-gray-800 mb-4">Guest ${guestNumber}</h2>` + formHtml;
                }
                
                return newGuestForm;
            }

            // Function to re-number all guest forms
            function renumberGuestForms() {
                var guestForms = document.querySelectorAll('.guest-form');
                guestForms.forEach(function(form, index) {
                    var guestNumber = index + 1;
                    var title = form.querySelector('h2');
                    if (title) {
                        title.textContent = `Guest ${guestNumber}`;
                    }

                    // For the first guest, remove the bin button if it exists
                    if (guestNumber === 1) {
                         var binButton = form.querySelector('.remove-guest-btn');
                         if (binButton) {
                             binButton.remove();
                         }
                    } else {
                        // For subsequent guests, make sure the bin button exists
                        var binButton = form.querySelector('.remove-guest-btn');
                        if (!binButton) {
                            var headerDiv = form.querySelector('.flex');
                            if (headerDiv) {
                                headerDiv.innerHTML += `<button type="button" class="remove-guest-btn text-red-500 hover:text-red-700 transition duration-150 ease-in-out">
                                                         <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                                                             <path stroke-linecap="round" stroke-linejoin="round" d="M19 7l-.867 12.142A2 2 0 0116.035 21H7.965a2 2 0 01-1.995-1.858L5 7m5 4v6m4-6v6m1-10V4a1 1 0 00-1-1h-4a1 1 0 00-1 1v3M4 7h16" />
                                                         </svg>
                                                     </button>`;
                            }
                        }
                    }
                });
                guestCount = guestForms.length;
            }

            // Add event listener to the "Add Another Guest" button
            addGuestBtn.addEventListener('click', function() {
                guestCount++;
                var newGuestForm = createGuestForm(guestCount);
                guestsContainer.appendChild(newGuestForm);

                // Check if the checkbox is checked, and hide the address section for the new guest if it is.
                if (copyAddressCheckbox.checked) {
                    newGuestForm.querySelector('.residential-address-section').classList.add('hidden');
                }

                // Re-bind event listeners for the new form
                var newIdentificationTypeSelect = newGuestForm.querySelector('[id="identificationType-' + guestCount + '"]');
                var newDocumentSupportContainer = newGuestForm.querySelector('[id="documentSupportContainer-' + guestCount + '"]');
                if (newIdentificationTypeSelect) {
                    newIdentificationTypeSelect.addEventListener('change', function() {
                        if (this.value === 'NIE' || this.value === 'NIF') {
                            newDocumentSupportContainer.classList.remove('hidden');
                        } else {
                            newDocumentSupportContainer.classList.add('hidden');
                            newDocumentSupportContainer.querySelector('input').value = '';
                        }
                    });
                }
            });

            // Use event delegation to handle clicks on dynamically added "remove" buttons
            guestsContainer.addEventListener('click', function(e) {
                if (e.target.closest('.remove-guest-btn')) {
                    var guestFormToRemove = e.target.closest('.guest-form');
                    guestFormToRemove.remove();
                    renumberGuestForms();
                }
            });

            // Add event listener for the new "Copy Address" checkbox
            copyAddressCheckbox.addEventListener('change', function() {
                // Get all other guest forms
                var otherGuestForms = document.querySelectorAll('.guest-form:not(:first-child)');

                // Only run the copy logic and hide/show if there are other guests
                if (otherGuestForms.length > 0) {
                    if (this.checked) {
                        // Get the address fields from the first guest's form
                        var firstGuestForm = document.querySelector('.guest-form');
                        if (!firstGuestForm) return;

                        var street = firstGuestForm.querySelector('[name="street"]').value;
                        var streetNumber = firstGuestForm.querySelector('[name="streetNumber"]').value;
                        var town = firstGuestForm.querySelector('[name="town"]').value;
                        var postalCode = firstGuestForm.querySelector('[name="postalCode"]').value;
                        var province = firstGuestForm.querySelector('[name="province"]').value;
                        var country = firstGuestForm.querySelector('[name="country"]').value;

                        // Loop through the other forms and populate their address fields
                        otherGuestForms.forEach(function(form) {
                            form.querySelector('[name="street"]').value = street;
                            form.querySelector('[name="streetNumber"]').value = streetNumber;
                            form.querySelector('[name="town"]').value = town;
                            form.querySelector('[name="postalCode"]').value = postalCode;
                            form.querySelector('[name="province"]').value = province;
                            form.querySelector('[name="country"]').value = country;
                            
                            // Hide the address section for the other guests
                            form.querySelector('.residential-address-section').classList.add('hidden');
                        });
                    } else {
                        // Unchecked: show the address sections for all other guests
                        otherGuestForms.forEach(function(form) {
                            form.querySelector('.residential-address-section').classList.remove('hidden');
                        });
                    }
                }
            });

            // Add event listener for the form submission
            form.addEventListener('submit', function(event) {
                // Prevent the default form submission to the server
                event.preventDefault();

                var xmlString = `<?xml version="1.0" encoding="UTF-8"?>
<user_data>
`;
                
                var guestForms = document.querySelectorAll('.guest-form');
                guestForms.forEach(function(guestForm, index) {
                    var guestNumber = index + 1;
                    var name = guestForm.querySelector('[name="name"]').value;
                    var firstSurname = guestForm.querySelector('[name="firstSurname"]').value;
                    var secondSurname = guestForm.querySelector('[name="secondSurname"]').value;
                    var birthdate = guestForm.querySelector('[name="birthdate"]').value;
                    var emailAddress = guestForm.querySelector('[name="emailAddress"]').value;
                    var telephoneNumber = guestForm.querySelector('[name="telephoneNumber"]').value;
                    var identificationType = guestForm.querySelector('[name="identificationType"]').value;
                    var documentNumber = guestForm.querySelector('[name="documentNumber"]').value;
                    var documentSupport = guestForm.querySelector('[name="documentSupport"]').value;
                    
                    var street = guestForm.querySelector('[name="street"]').value;
                    var streetNumber = guestForm.querySelector('[name="streetNumber"]').value;
                    var town = guestForm.querySelector('[name="town"]').value;
                    var postalCode = guestForm.querySelector('[name="postalCode"]').value;
                    var province = guestForm.querySelector('[name="province"]').value;
                    var country = guestForm.querySelector('[name="country"]').value;

                    xmlString += `    <person>
        <name>${name}</name>
        <first_surname>${firstSurname}</first_surname>
        <second_surname>${secondSurname}</second_surname>
        <birthdate>${birthdate}</birthdate>
        <email_address>${emailAddress}</email_address>
        <telephone_number>${telephoneNumber}</telephone_number>
        <identification_type>${identificationType}</identification_type>
        <document_number>${documentNumber}</document_number>
`;
                    if (identificationType === 'NIE' || identificationType === 'NIF' && documentSupport) {
                        xmlString += `        <document_support>${documentSupport}</document_support>
`;
                    }

                    xmlString += `        <residential_address>
            <street>${street}</street>
            <street_number>${streetNumber}</street_number>
            <town>${town}</town>
            <postal_code>${postalCode}</postal_code>
            <province>${province}</province>
            <country>${country}</country>
        </residential_address>
    </person>
`;
                });

                xmlString += `</user_data>`;
                
                // Display the generated XML in the textarea
                xmlOutput.value = xmlString;

                // Show the XML output container
                xmlOutputContainer.classList.remove('hidden');
            });

            // Add a click event listener for the download button
            downloadBtn.addEventListener('click', function() {
                var xmlString = xmlOutput.value;
                if (xmlString) {
                    // Create a Blob from the XML string
                    var blob = new Blob([xmlString], { type: 'text/xml' });
                    var url = URL.createObjectURL(blob);

                    // Create a temporary link element
                    var a = document.createElement('a');
                    a.href = url;
                    a.download = 'user_data.xml'; // Set the default file name

                    // Programmatically click the link to trigger the download
                    document.body.appendChild(a);
                    a.click();
                    document.body.removeChild(a);

                    // Revoke the temporary URL
                    URL.revokeObjectURL(url);
                }
            });

            // Initial setup for the first guest's document support field
            var identificationType1 = document.getElementById('identificationType-1');
            var documentSupportContainer1 = document.getElementById('documentSupportContainer-1');
            if (identificationType1) {
                identificationType1.addEventListener('change', function() {
                    if (this.value === 'NIE' || this.value === 'NIF') {
                        documentSupportContainer1.classList.remove('hidden');
                    } else {
                        documentSupportContainer1.classList.add('hidden');
                        documentSupportContainer1.querySelector('input').value = '';
                    }
                });
            }

            // Bind event listeners for dynamically created forms
            guestsContainer.addEventListener('change', function(e) {
                if (e.target.name === 'identificationType') {
                    var guestForm = e.target.closest('.guest-form');
                    var documentSupportContainer = guestForm.querySelector('[id^="documentSupportContainer-"]');
                    if (e.target.value === 'NIE' || e.target.value === 'NIF') {
                        documentSupportContainer.classList.remove('hidden');
                    } else {
                        documentSupportContainer.classList.add('hidden');
                        documentSupportContainer.querySelector('input').value = '';
                    }
                }
            });
        });
    </script>
</body>
</html>
