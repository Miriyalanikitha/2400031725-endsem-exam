# 2400031725-endsem-exam
import React from "react";
import EventCard from "./EventCard";

export default function App() {
  // Parent click handler
  const handleBookEvent = (eventName) => {
    alert(`You booked the event: ${eventName}`);
  };

  return (
    <div style={{ padding: "20px" }}>
      <h2>Event Booking Portal</h2>

      <EventCard
        title="Music Concert"
        onBook={() => handleBookEvent("Music Concert")}
      />

      <EventCard
        title="Tech Conference"
        onBook={() => handleBookEvent("Tech Conference")}
      />

      <EventCard
        title="Art Workshop"
        onBook={() => handleBookEvent("Art Workshop")}
      />
    </div>
  );
}
