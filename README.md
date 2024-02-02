# Room Booking Smart Contract

## Overview
This Solidity smart contract, `RoomBooking`, allows users to book rooms within a certain time frame and under specific conditions. It is designed to be deployed on the Ethereum blockchain.

## Features
- **Owner**: The contract maintains an owner, who has special privileges such as setting the booking limit and performing administrative actions.
- **Room Booking**: Users can book rooms by specifying the room number and booking time. Certain conditions must be met for a booking to be successful.
- **Booking Limit**: Each user has a predefined booking limit, preventing them from exceeding a certain number of bookings.
- **Modifiers**: The contract includes a modifier `onlyOwner` to restrict certain functions to be callable only by the owner.

## Functionality
- `constructor()`: Initializes the contract by setting the owner to the address that deployed the contract.
- `onlyOwner()`: Modifier to restrict access to functions only to the owner.
- `bookRoom(uint256 roomNumber, uint256 bookingTime)`: Allows users to book a room under specific conditions. Conditions include ensuring the booking time is between 1 AM to 6 AM and that the room number is divisible by 3.
- `getBookingCount(address user)`: Private function to retrieve the number of rooms booked by a specific user.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Author

Azamkhan

Azamkhan05071997@gmail.com
